---
title: 온라인 호스팅 지침
permalink: index.html
layout: home
ms.openlocfilehash: c612655617c9fb1f1baef2b3a78d0cb87f0e3d18
ms.sourcegitcommit: 525e69932921e8ce30e81ee0f98ad4a87cda64ea
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/18/2021
ms.locfileid: "137820816"
---
# <a name="content-directory"></a>콘텐츠 디렉터리

다음은 각 랩 연습 및 데모의 하이퍼링크입니다.

## <a name="labs"></a>랩

{% assign labs = site.pages | where_exp:"page", "page.url contains '/Instructions/Labs'" %}
| 모듈 | 랩 |
| --- | --- | 
{% for activity in labs  %}| {{ activity.lab.module }} | [{{ activity.lab.title }}{% if activity.lab.type %} - {{ activity.lab.type }}{% endif %}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}


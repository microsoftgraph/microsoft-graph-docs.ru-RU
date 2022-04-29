---
title: Сложный тип subjectSet
description: Абстрактный базовый тип для типов, используемых в параметрах проверки запросов, утверждений и назначений политики назначения пакетов доступа.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0a266aea0693c6faf994da0fd829b8cacdee619e
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133120"
---
# <a name="subjectset-complex-type"></a>Сложный тип subjectSet

Пространство имен: microsoft.graph

Общий объект, используемый в политиках назначения пакетов доступа для управления правами и политиках управления ролами.

+ В управлении правами используется в параметрах проверки запроса, утверждения и назначения политики назначения пакетов доступа.
+ В политиках управления ролами используется в параметрах утверждения, определенных в правилах для политик управления ролами.

Это абстрактный базовый тип, унаследованный следующими производными типами:
+ [singleUser](singleuser.md)
+ [singleServicePrincipal](singleserviceprincipal.md)
+ [groupMembers](groupmembers.md)
+ [connectedOrganizationMembers](connectedorganizationmembers.md)
+ [requestorManager](requestormanager.md)
+ [internalSponsors](internalsponsors.md)
+ [externalSponsors](externalsponsors.md)
+ [targetManager](targetmanager.md)
+ [targetApplicationOwners](targetapplicationowners.md)


## <a name="properties"></a>Свойства

Нет
## <a name="relationships"></a>Связи
Отсутствуют.
## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.subjectSet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.subjectSet"
}
```



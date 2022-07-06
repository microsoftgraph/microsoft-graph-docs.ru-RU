---
title: Тип ресурса synchronizationJobSubject
description: Представляет объекты, которые будут подготовлены во время подготовки по запросу.
author: ArvindHarinder1
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 33316bfb434d34c8f367832f9334938cf1c0cf8b
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645416"
---
# <a name="synchronizationjobsubject-resource-type"></a>Тип ресурса synchronizationJobSubject

Пространство имен: microsoft.graph

Представляет объекты, которые будут подготовлены во время подготовки по запросу.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|links|[synchronizationLinkedObjects](../resources/synchronization-synchronizationlinkedobjects.md)|Субъекты, которые вы хотите подготовить.|
|objectId|String|Идентификатор объекта, к которому будет **применено** задание синхронизации. Допустимые значения: <li>**OnPremisesDistinguishedName** для синхронизации из Active Directory в Azure AD.</li><li>Идентификатор пользователя для синхронизации от Azure AD к стороннему поставщику.</li><li>Идентификатор рабочей роли Workday для синхронизации из Workday в Active Directory или Azure AD.</li>|
|objectTypeName|String|Тип объекта, к которому будет **применено задание** синхронизации. Допустимые значения: <li>`user`для синхронизации между Active Directory и Azure AD.</li><li>`User`для синхронизации пользователя между Azure AD и сторонним приложением. </li><li>`Worker`для синхронизации пользователя между Workday и Active Directory или Azure AD.</li><li>`Group`для синхронизации группы между Azure AD и сторонним приложением. </li>|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationJobSubject"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationJobSubject",
  "objectId": "String",
  "objectTypeName": "String",
  "links": {
    "@odata.type": "microsoft.graph.synchronizationLinkedObjects"
  }
}
```



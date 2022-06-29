---
title: Тип ресурса synchronizationJobSubject
description: Представляет объекты, которые будут подготовлены во время подготовки по запросу.
author: ArvindHarinder1
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 2e6a0bea0f3e035bc5b0aef81a20b4a9dc480836
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441680"
---
# <a name="synchronizationjobsubject-resource-type"></a>Тип ресурса synchronizationJobSubject

Пространство имен: microsoft.graph

Представляет объекты, которые будут подготовлены во время подготовки по запросу.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|links|[synchronizationLinkedObjects](../resources/synchronizationlinkedobjects.md)|Субъекты, которые вы хотите подготовить.|
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



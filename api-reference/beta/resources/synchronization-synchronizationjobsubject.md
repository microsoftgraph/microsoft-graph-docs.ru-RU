---
title: Тип ресурса synchronizationJobSubject
description: Представляет объекты, которые будут подготовлены во время подготовки по запросу.
author: ArvindHarinder1
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: d9c19bc431ce152bb3b15f97822ee86071c314d8
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2022
ms.locfileid: "65061120"
---
# <a name="synchronizationjobsubject-resource-type"></a>Тип ресурса synchronizationJobSubject

Пространство имен: microsoft.graph

Представляет объекты, которые будут подготовлены во время подготовки по запросу.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|objectId|String|Идентификатор объекта, к которому будет **применено** задание синхронизации. Допустимые значения: <li>**OnPremisesDistinguishedName** для синхронизации из Active Directory в Azure AD.</li><li>Идентификатор пользователя для синхронизации из Azure AD со сторонним разработчиком.</li><li>Идентификатор рабочей роли Workday для синхронизации из Workday в Active Directory или Azure AD.</li>|
|objectTypeName|String|Тип объекта, к которому будет **применено задание** синхронизации. Допустимые значения: <li>`user` для синхронизации из Active Directory в Azure AD.</li><li>`User` для синхронизации из Azure AD в стороннее приложение. </li><li>`Worker` для синхронизации из Workday в Active Directory или Azure AD.</li>|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
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
  "objectTypeName": "String"
}
```



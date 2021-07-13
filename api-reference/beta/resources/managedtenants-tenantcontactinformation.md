---
title: тип ресурса tenantContactInformation
description: Представляет контакт в управляемом клиенте.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: b60005cf60a9ac1b96a3b650a853f8b198d27e48
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403157"
---
# <a name="tenantcontactinformation-resource-type"></a>тип ресурса tenantContactInformation

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет контакт в управляемом клиенте.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|email|String|Адрес электронной почты для контакта. Необязательный|
|name|String|Имя контакта. Обязательный.|
|notes|String|Заметки, связанные с контактом. Необязательный|
|phone|String|Номер телефона для контакта. Необязательное.|
|title|String|Название для контакта. Обязательный.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.tenantContactInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantContactInformation",
  "name": "String",
  "title": "String",
  "email": "String",
  "phone": "String",
  "notes": "String"
}
```

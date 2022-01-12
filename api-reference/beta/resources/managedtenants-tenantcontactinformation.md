---
title: тип ресурса tenantContactInformation
description: Представляет контакт в управляемом клиенте.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: f852bbae5a08c00d101e122443b9e5b50382eb62
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61860462"
---
# <a name="tenantcontactinformation-resource-type"></a>тип ресурса tenantContactInformation

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет контакт в управляемом клиенте.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|email|String|Адрес электронной почты для контакта. Необязательна|
|name|String|Имя контакта. Обязательный.|
|notes|String|Заметки, связанные с контактом. Необязательный|
|phone|String|Номер телефона для контакта. Необязательно.|
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

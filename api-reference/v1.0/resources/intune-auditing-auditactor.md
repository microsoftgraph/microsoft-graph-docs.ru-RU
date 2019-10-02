---
title: Тип ресурса auditActor
description: Класс, содержащий свойства субъекта аудита.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4365daebf50de210482132354c14199c850e384a
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355997"
---
# <a name="auditactor-resource-type"></a>Тип ресурса auditActor

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства субъекта аудита.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|type|String|Тип субъекта.|
|userPermissions|Коллекция строк|Список разрешений пользователей во время аудита.|
|applicationId|String|ИД приложения AAD.|
|applicationDisplayName|String|Имя приложения.|
|userPrincipalName|Строка|Имя участника-пользователя (UPN).|
|servicePrincipalName|String|Имя субъекта-службы (SPN).|
|ipAddress|String|IP-адрес.|
|userId|String|ИД пользователя.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditActor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditActor",
  "type": "String",
  "userPermissions": [
    "String"
  ],
  "applicationId": "String",
  "applicationDisplayName": "String",
  "userPrincipalName": "String",
  "servicePrincipalName": "String",
  "ipAddress": "String",
  "userId": "String"
}
```





---
title: Тип ресурса auditActor
description: Класс, содержащий свойства субъекта аудита.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0c10ac0a18f5bfcf68be56edc402c83d9882a8ff
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532735"
---
# <a name="auditactor-resource-type"></a>Тип ресурса auditActor

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства субъекта аудита.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|type|Строка|Тип субъекта.|
|userPermissions|Коллекция строк|Список разрешений пользователей во время аудита.|
|applicationId|Строка|ИД приложения AAD.|
|applicationDisplayName|Строка|Имя приложения.|
|userPrincipalName|Строка|Имя участника-пользователя (UPN).|
|servicePrincipalName|Строка|Имя субъекта-службы (SPN).|
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





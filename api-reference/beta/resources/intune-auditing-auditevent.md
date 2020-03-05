---
title: Тип ресурса auditEvent
description: Класс, содержащий свойства события аудита.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 392fa974fa29fd8619f15a99517413473fcdb28b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42489414"
---
# <a name="auditevent-resource-type"></a>Тип ресурса auditEvent

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства события аудита.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов auditEvent](../api/intune-auditing-auditevent-list.md)|Коллекция [auditEvent](../resources/intune-auditing-auditevent.md)|Список свойств и связей объектов [auditEvent](../resources/intune-auditing-auditevent.md).|
|[Получение объекта auditEvent](../api/intune-auditing-auditevent-get.md)|[auditEvent](../resources/intune-auditing-auditevent.md);|Чтение свойств и связей объекта [auditEvent](../resources/intune-auditing-auditevent.md).|
|[Создание объекта auditEvent](../api/intune-auditing-auditevent-create.md)|[auditEvent](../resources/intune-auditing-auditevent.md);|Создание объекта [auditEvent](../resources/intune-auditing-auditevent.md).|
|[Удаление объекта auditEvent](../api/intune-auditing-auditevent-delete.md)|Нет|Удаляет объект [auditEvent](../resources/intune-auditing-auditevent.md).|
|[Обновление объекта auditEvent](../api/intune-auditing-auditevent-update.md)|[auditEvent](../resources/intune-auditing-auditevent.md)|Обновление свойств объекта [auditEvent](../resources/intune-auditing-auditevent.md).|
|[Функция getAuditCategories](../api/intune-auditing-auditevent-getauditcategories.md)|Коллекция строк|Н/Д|
|[Функция getAuditActivityTypes](../api/intune-auditing-auditevent-getauditactivitytypes.md)|Коллекция строк|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|displayName|Строка|Отображаемое имя события.|
|componentName|String|Имя компонента.|
|actor|[auditActor](../resources/intune-auditing-auditactor.md)|Пользователь AAD и приложение, связанные с событием аудита.|
|activity|String|Понятное имя действия.|
|activityDateTime|DateTimeOffset|Дата и время выполнения действия (в формате UTC).|
|activityType|String|Тип выполненного действия.|
|activityOperationType|String|Тип операции HTTP для действия.|
|activityResult|String|Результат действия.|
|correlationId|Guid|ИД клиентского запроса, используемый для согласования действий в системе.|
|resources|Коллекция [auditResource](../resources/intune-auditing-auditresource.md)|Изменяемые ресурсы.|
|category|String|Категория аудита.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.auditEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditEvent",
  "id": "String (identifier)",
  "displayName": "String",
  "componentName": "String",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "String",
    "userPermissions": [
      "String"
    ],
    "applicationId": "String",
    "applicationDisplayName": "String",
    "userPrincipalName": "String",
    "servicePrincipalName": "String",
    "ipAddress": "String",
    "userId": "String",
    "userRoleScopeTags": [
      {
        "@odata.type": "microsoft.graph.roleScopeTagInfo",
        "displayName": "String",
        "roleScopeTagId": "String"
      }
    ]
  },
  "activity": "String",
  "activityDateTime": "String (timestamp)",
  "activityType": "String",
  "activityOperationType": "String",
  "activityResult": "String",
  "correlationId": "Guid",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource",
      "displayName": "String",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.auditProperty",
          "displayName": "String",
          "oldValue": "String",
          "newValue": "String"
        }
      ],
      "type": "String",
      "resourceId": "String"
    }
  ],
  "category": "String"
}
```




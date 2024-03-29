---
title: Тип ресурса auditEvent
description: Класс, содержащий свойства события аудита.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9750f450d31b4b1c9458fb941aafa8bdf8a6018d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091820"
---
# <a name="auditevent-resource-type"></a>Тип ресурса auditEvent

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства события аудита.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов auditEvent](../api/intune-auditing-auditevent-list.md)|Коллекция [auditEvent](../resources/intune-auditing-auditevent.md)|Список свойств и связей объектов [auditEvent](../resources/intune-auditing-auditevent.md).|
|[Получение объекта auditEvent](../api/intune-auditing-auditevent-get.md)|[auditEvent](../resources/intune-auditing-auditevent.md)|Чтение свойств и связей объекта [auditEvent](../resources/intune-auditing-auditevent.md).|
|[Создание объекта auditEvent](../api/intune-auditing-auditevent-create.md)|[auditEvent](../resources/intune-auditing-auditevent.md)|Создание объекта [auditEvent](../resources/intune-auditing-auditevent.md).|
|[Удаление объекта auditEvent](../api/intune-auditing-auditevent-delete.md)|Нет|Удаляет объект [auditEvent](../resources/intune-auditing-auditevent.md).|
|[Обновление объекта auditEvent](../api/intune-auditing-auditevent-update.md)|[auditEvent](../resources/intune-auditing-auditevent.md)|Обновление свойств объекта [auditEvent](../resources/intune-auditing-auditevent.md).|
|[Функция getAuditCategories](../api/intune-auditing-auditevent-getauditcategories.md)|Коллекция строк|Н/Д|
|[Функция getAuditActivityTypes](../api/intune-auditing-auditevent-getauditactivitytypes.md)|Коллекция строк|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|displayName|String|Отображаемое имя события.|
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
    ],
    "remoteTenantId": "String",
    "remoteUserId": "String"
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




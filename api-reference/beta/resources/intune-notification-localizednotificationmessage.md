---
title: Тип ресурса localizedNotificationMessage
description: Текстовое содержимое шаблона сообщения уведомления для указанного языкового стандарта.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 29c8da43ded157ada25488c299ac27c25dd7cd56
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967821"
---
# <a name="localizednotificationmessage-resource-type"></a>Тип ресурса localizedNotificationMessage

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Текстовое содержимое шаблона сообщения уведомления для указанного языкового стандарта.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов localizedNotificationMessage](../api/intune-notification-localizednotificationmessage-list.md)|Коллекция [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)|Список свойств и связей объектов [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).|
|[Получение объекта localizedNotificationMessage](../api/intune-notification-localizednotificationmessage-get.md)|[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md);|Чтение свойств и связей объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).|
|[Создание объекта localizedNotificationMessage](../api/intune-notification-localizednotificationmessage-create.md)|[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md);|Создание объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).|
|[Удаление объекта localizedNotificationMessage](../api/intune-notification-localizednotificationmessage-delete.md)|Нет|Удаляет объект [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).|
|[Обновление объекта localizedNotificationMessage](../api/intune-notification-localizednotificationmessage-update.md)|[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)|Обновление свойств объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|
|locale|String|Языковой стандарт, для которого предназначено сообщение.|
|subject|String|Тема шаблона сообщения.|
|messageTemplate|String|Содержимое шаблона сообщения.|
|isDefault|Boolean|Флаг, указывающий, используется ли этот языковой стандарт в качестве базового языка. Можно устанавливать только этот флаг. Чтобы снять его, задайте значение true для аналогичного свойства другого локализованного сообщения уведомления.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.localizedNotificationMessage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "locale": "String",
  "subject": "String",
  "messageTemplate": "String",
  "isDefault": true
}
```






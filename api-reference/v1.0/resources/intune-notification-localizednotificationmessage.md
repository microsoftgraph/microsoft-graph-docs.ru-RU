---
title: Тип ресурса localizedNotificationMessage
description: Текстовое содержимое шаблона сообщения уведомления для указанного языкового стандарта.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 403952300d9072072b99f0dd58aa56e32ca22d69
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755716"
---
# <a name="localizednotificationmessage-resource-type"></a>Тип ресурса localizedNotificationMessage

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Текстовое содержимое шаблона сообщения уведомления для указанного языкового стандарта.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов localizedNotificationMessage](../api/intune-notification-localizednotificationmessage-list.md)|Коллекция [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)|Список свойств и связей объектов [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).|
|[Получение объекта localizedNotificationMessage](../api/intune-notification-localizednotificationmessage-get.md)|[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)|Чтение свойств и связей объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).|
|[Создание объекта localizedNotificationMessage](../api/intune-notification-localizednotificationmessage-create.md)|[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)|Создание объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).|
|[Удаление объекта localizedNotificationMessage](../api/intune-notification-localizednotificationmessage-delete.md)|Нет|Удаляет объект [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).|
|[Обновление объекта localizedNotificationMessage](../api/intune-notification-localizednotificationmessage-update.md)|[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)|Обновление свойств объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
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





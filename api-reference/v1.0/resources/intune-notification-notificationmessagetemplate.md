---
title: Тип ресурса notificationMessageTemplate
description: Сообщения уведомлений отправляются пользователям, которые не отвечают политикам соответствия требованиям, определяемым администратором. Администраторы выбирают уведомления и настраивают их в консоли администрирования Intune, используя страницу создания политики соответствия требованиям в разделе "Действия для несоответствия". Используйте объект notificationMessageTemplate, чтобы создать собственные настраиваемые уведомления, которые могут выбрать администраторы во время настройки действий в случае несоответствия требованиям.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e534045abda83013443c06fbdfdd63bfe68cae84
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66729897"
---
# <a name="notificationmessagetemplate-resource-type"></a>Тип ресурса notificationMessageTemplate

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сообщения уведомлений отправляются пользователям, которые не отвечают политикам соответствия требованиям, определяемым администратором. Администраторы выбирают уведомления и настраивают их в консоли администрирования Intune, используя страницу создания политики соответствия требованиям в разделе "Действия для несоответствия". Используйте объект notificationMessageTemplate, чтобы создать собственные настраиваемые уведомления, которые могут выбрать администраторы во время настройки действий в случае несоответствия требованиям.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов notificationMessageTemplate](../api/intune-notification-notificationmessagetemplate-list.md)|Коллекция объектов [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|Список свойств и связей объектов [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).|
|[Получение объекта notificationMessageTemplate](../api/intune-notification-notificationmessagetemplate-get.md)|[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|Чтение свойств и связей объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).|
|[Создание объекта notificationMessageTemplate](../api/intune-notification-notificationmessagetemplate-create.md)|[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|Создание объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).|
|[Удаление объекта notificationMessageTemplate](../api/intune-notification-notificationmessagetemplate-delete.md)|Нет|Удаление объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).|
|[Обновление объекта notificationMessageTemplate](../api/intune-notification-notificationmessagetemplate-update.md)|[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)|Обновление свойств объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).|
|[Действие sendTestMessage](../api/intune-notification-notificationmessagetemplate-sendtestmessage.md)|Нет|Отправляет проверочное сообщение, используя объект notificationMessageTemplate, указанный в языковом стандарте по умолчанию.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|
|displayName|String|Отображаемое имя для шаблона сообщения уведомления.|
|defaultLocale|String|Языковой стандарт по умолчанию, который используется, если запрошенный языковой стандарт недоступен.|
|brandingOptions|[notificationTemplateBrandingOptions](../resources/intune-notification-notificationtemplatebrandingoptions.md)|Параметры фирменной символики шаблона сообщения. Фирменная символика определяется в консоли администрирования Intune. Возможные значения: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`, `includeDeviceDetails`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|localizedNotificationMessages|Коллекция объектов [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)|Список локализованных сообщений для шаблона сообщения уведомления.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.notificationMessageTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "defaultLocale": "String",
  "brandingOptions": "String"
}
```






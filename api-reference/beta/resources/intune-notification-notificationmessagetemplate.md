---
title: Тип ресурса notificationMessageTemplate
description: Сообщения уведомлений отправляются пользователям, которые не отвечают политикам соответствия требованиям, определяемым администратором. Администраторы выбирают уведомления и настраивают их в консоли администрирования Intune, используя страницу создания политики соответствия требованиям в разделе "Действия для несоответствия". Используйте объект notificationMessageTemplate, чтобы создать собственные настраиваемые уведомления, которые могут выбрать администраторы во время настройки действий в случае несоответствия требованиям.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5b76ddbc9f55f1129cb186b23022812c84ce32a7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394784"
---
# <a name="notificationmessagetemplate-resource-type"></a>Тип ресурса notificationMessageTemplate

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|brandingOptions|[notificationTemplateBrandingOptions](../resources/intune-notification-notificationtemplatebrandingoptions.md)|Параметры фирменной символики шаблона сообщения. Фирменная символика определяется в консоли администрирования Intune. Возможные значения: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.|
|roleScopeTagIds|Коллекция String|Список областей теги для данного экземпляра сущности.|

## <a name="relationships"></a>Отношения
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
  "brandingOptions": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```





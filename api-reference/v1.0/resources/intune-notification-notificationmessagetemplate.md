---
title: Тип ресурса notificationMessageTemplate
description: Сообщения уведомлений отправляются пользователям, которые не отвечают политикам соответствия требованиям, определяемым администратором. Администраторы выбирают уведомления и настраивают их в консоли администрирования Intune, используя страницу создания политики соответствия требованиям в разделе "Действия для несоответствия". Используйте объект notificationMessageTemplate, чтобы создать собственные настраиваемые уведомления, которые могут выбрать администраторы во время настройки действий в случае несоответствия требованиям.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 05db5042b43097f0ff48f4c744e3b4bcd82f691d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072993"
---
# <a name="notificationmessagetemplate-resource-type"></a><span data-ttu-id="c0217-105">Тип ресурса notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="c0217-105">notificationMessageTemplate resource type</span></span>

<span data-ttu-id="c0217-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0217-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0217-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c0217-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0217-108">Сообщения уведомлений отправляются пользователям, которые не отвечают политикам соответствия требованиям, определяемым администратором.</span><span class="sxs-lookup"><span data-stu-id="c0217-108">Notification messages are messages that are sent to end users who are determined to be not-compliant with the compliance policies defined by the administrator.</span></span> <span data-ttu-id="c0217-109">Администраторы выбирают уведомления и настраивают их в консоли администрирования Intune, используя страницу создания политики соответствия требованиям в разделе "Действия для несоответствия".</span><span class="sxs-lookup"><span data-stu-id="c0217-109">Administrators choose notifications and configure them in the Intune Admin Console using the compliance policy creation page under the “Actions for non-compliance” section.</span></span> <span data-ttu-id="c0217-110">Используйте объект notificationMessageTemplate, чтобы создать собственные настраиваемые уведомления, которые могут выбрать администраторы во время настройки действий в случае несоответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="c0217-110">Use the notificationMessageTemplate object to create your own custom notifications for administrators to choose while configuring actions for non-compliance.</span></span>

## <a name="methods"></a><span data-ttu-id="c0217-111">Методы</span><span class="sxs-lookup"><span data-stu-id="c0217-111">Methods</span></span>
|<span data-ttu-id="c0217-112">Метод</span><span class="sxs-lookup"><span data-stu-id="c0217-112">Method</span></span>|<span data-ttu-id="c0217-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c0217-113">Return Type</span></span>|<span data-ttu-id="c0217-114">Описание</span><span class="sxs-lookup"><span data-stu-id="c0217-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c0217-115">Перечисление объектов notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="c0217-115">List notificationMessageTemplates</span></span>](../api/intune-notification-notificationmessagetemplate-list.md)|<span data-ttu-id="c0217-116">Коллекция объектов [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="c0217-116">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) collection</span></span>|<span data-ttu-id="c0217-117">Список свойств и связей объектов [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="c0217-117">List properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects.</span></span>|
|[<span data-ttu-id="c0217-118">Получение объекта notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="c0217-118">Get notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-get.md)|[<span data-ttu-id="c0217-119">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="c0217-119">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="c0217-120">Чтение свойств и связей объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="c0217-120">Read properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="c0217-121">Создание объекта notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="c0217-121">Create notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-create.md)|[<span data-ttu-id="c0217-122">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="c0217-122">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="c0217-123">Создание объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="c0217-123">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="c0217-124">Удаление объекта notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="c0217-124">Delete notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-delete.md)|<span data-ttu-id="c0217-125">Нет</span><span class="sxs-lookup"><span data-stu-id="c0217-125">None</span></span>|<span data-ttu-id="c0217-126">Удаление объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="c0217-126">Deletes a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>|
|[<span data-ttu-id="c0217-127">Обновление объекта notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="c0217-127">Update notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-update.md)|[<span data-ttu-id="c0217-128">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="c0217-128">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="c0217-129">Обновление свойств объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="c0217-129">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="c0217-130">Действие sendTestMessage</span><span class="sxs-lookup"><span data-stu-id="c0217-130">sendTestMessage action</span></span>](../api/intune-notification-notificationmessagetemplate-sendtestmessage.md)|<span data-ttu-id="c0217-131">Нет</span><span class="sxs-lookup"><span data-stu-id="c0217-131">None</span></span>|<span data-ttu-id="c0217-132">Отправляет проверочное сообщение, используя объект notificationMessageTemplate, указанный в языковом стандарте по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c0217-132">Sends test message using the specified notificationMessageTemplate in the default locale</span></span>|

## <a name="properties"></a><span data-ttu-id="c0217-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="c0217-133">Properties</span></span>
|<span data-ttu-id="c0217-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0217-134">Property</span></span>|<span data-ttu-id="c0217-135">Тип</span><span class="sxs-lookup"><span data-stu-id="c0217-135">Type</span></span>|<span data-ttu-id="c0217-136">Описание</span><span class="sxs-lookup"><span data-stu-id="c0217-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0217-137">id</span><span class="sxs-lookup"><span data-stu-id="c0217-137">id</span></span>|<span data-ttu-id="c0217-138">Строка</span><span class="sxs-lookup"><span data-stu-id="c0217-138">String</span></span>|<span data-ttu-id="c0217-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c0217-139">Key of the entity.</span></span>|
|<span data-ttu-id="c0217-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c0217-140">lastModifiedDateTime</span></span>|<span data-ttu-id="c0217-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0217-141">DateTimeOffset</span></span>|<span data-ttu-id="c0217-142">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c0217-142">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="c0217-143">displayName</span><span class="sxs-lookup"><span data-stu-id="c0217-143">displayName</span></span>|<span data-ttu-id="c0217-144">Строка</span><span class="sxs-lookup"><span data-stu-id="c0217-144">String</span></span>|<span data-ttu-id="c0217-145">Отображаемое имя для шаблона сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="c0217-145">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="c0217-146">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="c0217-146">defaultLocale</span></span>|<span data-ttu-id="c0217-147">String</span><span class="sxs-lookup"><span data-stu-id="c0217-147">String</span></span>|<span data-ttu-id="c0217-148">Языковой стандарт по умолчанию, который используется, если запрошенный языковой стандарт недоступен.</span><span class="sxs-lookup"><span data-stu-id="c0217-148">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="c0217-149">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="c0217-149">brandingOptions</span></span>|[<span data-ttu-id="c0217-150">нотификатионтемплатебрандингоптионс</span><span class="sxs-lookup"><span data-stu-id="c0217-150">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="c0217-151">Параметры фирменной символики шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="c0217-151">The Message Template Branding Options.</span></span> <span data-ttu-id="c0217-152">Фирменная символика определяется в консоли администрирования Intune.</span><span class="sxs-lookup"><span data-stu-id="c0217-152">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="c0217-153">Возможные значения: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="c0217-153">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0217-154">Связи</span><span class="sxs-lookup"><span data-stu-id="c0217-154">Relationships</span></span>
|<span data-ttu-id="c0217-155">Связь</span><span class="sxs-lookup"><span data-stu-id="c0217-155">Relationship</span></span>|<span data-ttu-id="c0217-156">Тип</span><span class="sxs-lookup"><span data-stu-id="c0217-156">Type</span></span>|<span data-ttu-id="c0217-157">Описание</span><span class="sxs-lookup"><span data-stu-id="c0217-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0217-158">localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="c0217-158">localizedNotificationMessages</span></span>|<span data-ttu-id="c0217-159">Коллекция объектов [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)</span><span class="sxs-lookup"><span data-stu-id="c0217-159">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) collection</span></span>|<span data-ttu-id="c0217-160">Список локализованных сообщений для шаблона сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="c0217-160">The list of localized messages for this Notification Message Template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c0217-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c0217-161">JSON Representation</span></span>
<span data-ttu-id="c0217-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c0217-162">Here is a JSON representation of the resource.</span></span>
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










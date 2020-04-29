---
title: Тип ресурса notificationMessageTemplate
description: Сообщения уведомлений отправляются пользователям, которые не отвечают политикам соответствия требованиям, определяемым администратором. Администраторы выбирают уведомления и настраивают их в консоли администрирования Intune, используя страницу создания политики соответствия требованиям в разделе "Действия для несоответствия". Используйте объект notificationMessageTemplate, чтобы создать собственные настраиваемые уведомления, которые могут выбрать администраторы во время настройки действий в случае несоответствия требованиям.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bdc400a84f51fa11f3d70b28fd21973fd1cf663c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459627"
---
# <a name="notificationmessagetemplate-resource-type"></a><span data-ttu-id="f958e-105">Тип ресурса notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="f958e-105">notificationMessageTemplate resource type</span></span>

<span data-ttu-id="f958e-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f958e-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f958e-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f958e-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f958e-108">Сообщения уведомлений отправляются пользователям, которые не отвечают политикам соответствия требованиям, определяемым администратором.</span><span class="sxs-lookup"><span data-stu-id="f958e-108">Notification messages are messages that are sent to end users who are determined to be not-compliant with the compliance policies defined by the administrator.</span></span> <span data-ttu-id="f958e-109">Администраторы выбирают уведомления и настраивают их в консоли администрирования Intune, используя страницу создания политики соответствия требованиям в разделе "Действия для несоответствия".</span><span class="sxs-lookup"><span data-stu-id="f958e-109">Administrators choose notifications and configure them in the Intune Admin Console using the compliance policy creation page under the “Actions for non-compliance” section.</span></span> <span data-ttu-id="f958e-110">Используйте объект notificationMessageTemplate, чтобы создать собственные настраиваемые уведомления, которые могут выбрать администраторы во время настройки действий в случае несоответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="f958e-110">Use the notificationMessageTemplate object to create your own custom notifications for administrators to choose while configuring actions for non-compliance.</span></span>

## <a name="methods"></a><span data-ttu-id="f958e-111">Методы</span><span class="sxs-lookup"><span data-stu-id="f958e-111">Methods</span></span>
|<span data-ttu-id="f958e-112">Метод</span><span class="sxs-lookup"><span data-stu-id="f958e-112">Method</span></span>|<span data-ttu-id="f958e-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f958e-113">Return Type</span></span>|<span data-ttu-id="f958e-114">Описание</span><span class="sxs-lookup"><span data-stu-id="f958e-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f958e-115">Перечисление объектов notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="f958e-115">List notificationMessageTemplates</span></span>](../api/intune-notification-notificationmessagetemplate-list.md)|<span data-ttu-id="f958e-116">Коллекция объектов [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="f958e-116">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) collection</span></span>|<span data-ttu-id="f958e-117">Список свойств и связей объектов [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="f958e-117">List properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects.</span></span>|
|[<span data-ttu-id="f958e-118">Получение объекта notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="f958e-118">Get notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-get.md)|<span data-ttu-id="f958e-119">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md);</span><span class="sxs-lookup"><span data-stu-id="f958e-119">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)</span></span>|<span data-ttu-id="f958e-120">Чтение свойств и связей объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="f958e-120">Read properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="f958e-121">Создание объекта notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="f958e-121">Create notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-create.md)|<span data-ttu-id="f958e-122">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md);</span><span class="sxs-lookup"><span data-stu-id="f958e-122">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)</span></span>|<span data-ttu-id="f958e-123">Создание объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="f958e-123">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="f958e-124">Удаление объекта notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="f958e-124">Delete notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-delete.md)|<span data-ttu-id="f958e-125">Нет</span><span class="sxs-lookup"><span data-stu-id="f958e-125">None</span></span>|<span data-ttu-id="f958e-126">Удаление объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="f958e-126">Deletes a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>|
|[<span data-ttu-id="f958e-127">Обновление объекта notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="f958e-127">Update notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-update.md)|[<span data-ttu-id="f958e-128">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="f958e-128">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="f958e-129">Обновление свойств объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="f958e-129">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="f958e-130">Действие sendTestMessage</span><span class="sxs-lookup"><span data-stu-id="f958e-130">sendTestMessage action</span></span>](../api/intune-notification-notificationmessagetemplate-sendtestmessage.md)|<span data-ttu-id="f958e-131">Нет</span><span class="sxs-lookup"><span data-stu-id="f958e-131">None</span></span>|<span data-ttu-id="f958e-132">Отправляет проверочное сообщение, используя объект notificationMessageTemplate, указанный в языковом стандарте по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f958e-132">Sends test message using the specified notificationMessageTemplate in the default locale</span></span>|

## <a name="properties"></a><span data-ttu-id="f958e-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="f958e-133">Properties</span></span>
|<span data-ttu-id="f958e-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="f958e-134">Property</span></span>|<span data-ttu-id="f958e-135">Тип</span><span class="sxs-lookup"><span data-stu-id="f958e-135">Type</span></span>|<span data-ttu-id="f958e-136">Описание</span><span class="sxs-lookup"><span data-stu-id="f958e-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f958e-137">id</span><span class="sxs-lookup"><span data-stu-id="f958e-137">id</span></span>|<span data-ttu-id="f958e-138">String</span><span class="sxs-lookup"><span data-stu-id="f958e-138">String</span></span>|<span data-ttu-id="f958e-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f958e-139">Key of the entity.</span></span>|
|<span data-ttu-id="f958e-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f958e-140">lastModifiedDateTime</span></span>|<span data-ttu-id="f958e-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f958e-141">DateTimeOffset</span></span>|<span data-ttu-id="f958e-142">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f958e-142">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="f958e-143">displayName</span><span class="sxs-lookup"><span data-stu-id="f958e-143">displayName</span></span>|<span data-ttu-id="f958e-144">Строка</span><span class="sxs-lookup"><span data-stu-id="f958e-144">String</span></span>|<span data-ttu-id="f958e-145">Отображаемое имя для шаблона сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="f958e-145">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="f958e-146">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="f958e-146">defaultLocale</span></span>|<span data-ttu-id="f958e-147">String</span><span class="sxs-lookup"><span data-stu-id="f958e-147">String</span></span>|<span data-ttu-id="f958e-148">Языковой стандарт по умолчанию, который используется, если запрошенный языковой стандарт недоступен.</span><span class="sxs-lookup"><span data-stu-id="f958e-148">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="f958e-149">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="f958e-149">brandingOptions</span></span>|[<span data-ttu-id="f958e-150">нотификатионтемплатебрандингоптионс</span><span class="sxs-lookup"><span data-stu-id="f958e-150">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="f958e-151">Параметры фирменной символики шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="f958e-151">The Message Template Branding Options.</span></span> <span data-ttu-id="f958e-152">Фирменная символика определяется в консоли администрирования Intune.</span><span class="sxs-lookup"><span data-stu-id="f958e-152">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="f958e-153">Возможные значения: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="f958e-153">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f958e-154">Связи</span><span class="sxs-lookup"><span data-stu-id="f958e-154">Relationships</span></span>
|<span data-ttu-id="f958e-155">Связь</span><span class="sxs-lookup"><span data-stu-id="f958e-155">Relationship</span></span>|<span data-ttu-id="f958e-156">Тип</span><span class="sxs-lookup"><span data-stu-id="f958e-156">Type</span></span>|<span data-ttu-id="f958e-157">Описание</span><span class="sxs-lookup"><span data-stu-id="f958e-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f958e-158">localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="f958e-158">localizedNotificationMessages</span></span>|<span data-ttu-id="f958e-159">Коллекция объектов [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)</span><span class="sxs-lookup"><span data-stu-id="f958e-159">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) collection</span></span>|<span data-ttu-id="f958e-160">Список локализованных сообщений для шаблона сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="f958e-160">The list of localized messages for this Notification Message Template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f958e-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f958e-161">JSON Representation</span></span>
<span data-ttu-id="f958e-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f958e-162">Here is a JSON representation of the resource.</span></span>
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








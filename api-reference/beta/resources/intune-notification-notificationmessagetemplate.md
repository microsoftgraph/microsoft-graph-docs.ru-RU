---
title: Тип ресурса notificationMessageTemplate
description: Сообщения уведомлений отправляются пользователям, которые не отвечают политикам соответствия требованиям, определяемым администратором. Администраторы выбирают уведомления и настраивают их в консоли администрирования Intune, используя страницу создания политики соответствия требованиям в разделе "Действия для несоответствия". Используйте объект notificationMessageTemplate, чтобы создать собственные настраиваемые уведомления, которые могут выбрать администраторы во время настройки действий в случае несоответствия требованиям.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9c4e0c2f7cfe723d8e8ac2ec5b583889aa2e6602
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029892"
---
# <a name="notificationmessagetemplate-resource-type"></a><span data-ttu-id="89ddf-105">Тип ресурса notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="89ddf-105">notificationMessageTemplate resource type</span></span>

<span data-ttu-id="89ddf-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89ddf-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89ddf-107">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89ddf-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89ddf-108">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="89ddf-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89ddf-109">Сообщения уведомлений отправляются пользователям, которые не отвечают политикам соответствия требованиям, определяемым администратором.</span><span class="sxs-lookup"><span data-stu-id="89ddf-109">Notification messages are messages that are sent to end users who are determined to be not-compliant with the compliance policies defined by the administrator.</span></span> <span data-ttu-id="89ddf-110">Администраторы выбирают уведомления и настраивают их в консоли администрирования Intune, используя страницу создания политики соответствия требованиям в разделе "Действия для несоответствия".</span><span class="sxs-lookup"><span data-stu-id="89ddf-110">Administrators choose notifications and configure them in the Intune Admin Console using the compliance policy creation page under the “Actions for non-compliance” section.</span></span> <span data-ttu-id="89ddf-111">Используйте объект notificationMessageTemplate, чтобы создать собственные настраиваемые уведомления, которые могут выбрать администраторы во время настройки действий в случае несоответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="89ddf-111">Use the notificationMessageTemplate object to create your own custom notifications for administrators to choose while configuring actions for non-compliance.</span></span>

## <a name="methods"></a><span data-ttu-id="89ddf-112">Методы</span><span class="sxs-lookup"><span data-stu-id="89ddf-112">Methods</span></span>
|<span data-ttu-id="89ddf-113">Метод</span><span class="sxs-lookup"><span data-stu-id="89ddf-113">Method</span></span>|<span data-ttu-id="89ddf-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="89ddf-114">Return Type</span></span>|<span data-ttu-id="89ddf-115">Описание</span><span class="sxs-lookup"><span data-stu-id="89ddf-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="89ddf-116">Перечисление объектов notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="89ddf-116">List notificationMessageTemplates</span></span>](../api/intune-notification-notificationmessagetemplate-list.md)|<span data-ttu-id="89ddf-117">Коллекция объектов [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="89ddf-117">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) collection</span></span>|<span data-ttu-id="89ddf-118">Список свойств и связей объектов [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="89ddf-118">List properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects.</span></span>|
|[<span data-ttu-id="89ddf-119">Получение объекта notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="89ddf-119">Get notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-get.md)|[<span data-ttu-id="89ddf-120">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="89ddf-120">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="89ddf-121">Чтение свойств и связей объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="89ddf-121">Read properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="89ddf-122">Создание объекта notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="89ddf-122">Create notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-create.md)|[<span data-ttu-id="89ddf-123">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="89ddf-123">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="89ddf-124">Создание объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="89ddf-124">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="89ddf-125">Удаление объекта notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="89ddf-125">Delete notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-delete.md)|<span data-ttu-id="89ddf-126">Нет</span><span class="sxs-lookup"><span data-stu-id="89ddf-126">None</span></span>|<span data-ttu-id="89ddf-127">Удаление объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="89ddf-127">Deletes a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>|
|[<span data-ttu-id="89ddf-128">Обновление объекта notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="89ddf-128">Update notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-update.md)|[<span data-ttu-id="89ddf-129">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="89ddf-129">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="89ddf-130">Обновление свойств объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="89ddf-130">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="89ddf-131">Действие sendTestMessage</span><span class="sxs-lookup"><span data-stu-id="89ddf-131">sendTestMessage action</span></span>](../api/intune-notification-notificationmessagetemplate-sendtestmessage.md)|<span data-ttu-id="89ddf-132">Нет</span><span class="sxs-lookup"><span data-stu-id="89ddf-132">None</span></span>|<span data-ttu-id="89ddf-133">Отправляет проверочное сообщение, используя объект notificationMessageTemplate, указанный в языковом стандарте по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="89ddf-133">Sends test message using the specified notificationMessageTemplate in the default locale</span></span>|

## <a name="properties"></a><span data-ttu-id="89ddf-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="89ddf-134">Properties</span></span>
|<span data-ttu-id="89ddf-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="89ddf-135">Property</span></span>|<span data-ttu-id="89ddf-136">Тип</span><span class="sxs-lookup"><span data-stu-id="89ddf-136">Type</span></span>|<span data-ttu-id="89ddf-137">Описание</span><span class="sxs-lookup"><span data-stu-id="89ddf-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89ddf-138">id</span><span class="sxs-lookup"><span data-stu-id="89ddf-138">id</span></span>|<span data-ttu-id="89ddf-139">String</span><span class="sxs-lookup"><span data-stu-id="89ddf-139">String</span></span>|<span data-ttu-id="89ddf-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="89ddf-140">Key of the entity.</span></span>|
|<span data-ttu-id="89ddf-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="89ddf-141">lastModifiedDateTime</span></span>|<span data-ttu-id="89ddf-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89ddf-142">DateTimeOffset</span></span>|<span data-ttu-id="89ddf-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="89ddf-143">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="89ddf-144">displayName</span><span class="sxs-lookup"><span data-stu-id="89ddf-144">displayName</span></span>|<span data-ttu-id="89ddf-145">String</span><span class="sxs-lookup"><span data-stu-id="89ddf-145">String</span></span>|<span data-ttu-id="89ddf-146">Отображаемое имя для шаблона сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="89ddf-146">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="89ddf-147">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="89ddf-147">defaultLocale</span></span>|<span data-ttu-id="89ddf-148">String</span><span class="sxs-lookup"><span data-stu-id="89ddf-148">String</span></span>|<span data-ttu-id="89ddf-149">Языковой стандарт по умолчанию, который используется, если запрошенный языковой стандарт недоступен.</span><span class="sxs-lookup"><span data-stu-id="89ddf-149">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="89ddf-150">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="89ddf-150">brandingOptions</span></span>|[<span data-ttu-id="89ddf-151">нотификатионтемплатебрандингоптионс</span><span class="sxs-lookup"><span data-stu-id="89ddf-151">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="89ddf-152">Параметры фирменной символики шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="89ddf-152">The Message Template Branding Options.</span></span> <span data-ttu-id="89ddf-153">Фирменная символика определяется в консоли администрирования Intune.</span><span class="sxs-lookup"><span data-stu-id="89ddf-153">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="89ddf-154">Возможные значения: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`, `includeCompanyPortalLink`.</span><span class="sxs-lookup"><span data-stu-id="89ddf-154">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`, `includeCompanyPortalLink`.</span></span>|
|<span data-ttu-id="89ddf-155">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="89ddf-155">roleScopeTagIds</span></span>|<span data-ttu-id="89ddf-156">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="89ddf-156">String collection</span></span>|<span data-ttu-id="89ddf-157">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="89ddf-157">List of Scope Tags for this Entity instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="89ddf-158">Отношения</span><span class="sxs-lookup"><span data-stu-id="89ddf-158">Relationships</span></span>
|<span data-ttu-id="89ddf-159">Связь</span><span class="sxs-lookup"><span data-stu-id="89ddf-159">Relationship</span></span>|<span data-ttu-id="89ddf-160">Тип</span><span class="sxs-lookup"><span data-stu-id="89ddf-160">Type</span></span>|<span data-ttu-id="89ddf-161">Описание</span><span class="sxs-lookup"><span data-stu-id="89ddf-161">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89ddf-162">localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="89ddf-162">localizedNotificationMessages</span></span>|<span data-ttu-id="89ddf-163">Коллекция объектов [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)</span><span class="sxs-lookup"><span data-stu-id="89ddf-163">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) collection</span></span>|<span data-ttu-id="89ddf-164">Список локализованных сообщений для шаблона сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="89ddf-164">The list of localized messages for this Notification Message Template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="89ddf-165">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="89ddf-165">JSON Representation</span></span>
<span data-ttu-id="89ddf-166">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89ddf-166">Here is a JSON representation of the resource.</span></span>
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







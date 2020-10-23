---
title: Обновление объекта notificationMessageTemplate
description: Обновление свойств объекта notificationMessageTemplate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 193865dcacf8b1f4cf10227786a8c29e8caa4374
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727726"
---
# <a name="update-notificationmessagetemplate"></a><span data-ttu-id="63346-103">Обновление объекта notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="63346-103">Update notificationMessageTemplate</span></span>

<span data-ttu-id="63346-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63346-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63346-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63346-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63346-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="63346-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63346-107">Обновление свойств объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="63346-107">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63346-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="63346-108">Prerequisites</span></span>
<span data-ttu-id="63346-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63346-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63346-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63346-111">Permission type</span></span>|<span data-ttu-id="63346-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="63346-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63346-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63346-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63346-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63346-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="63346-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63346-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63346-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63346-116">Not supported.</span></span>|
|<span data-ttu-id="63346-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="63346-117">Application</span></span>|<span data-ttu-id="63346-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63346-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="63346-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63346-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="63346-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="63346-120">Request headers</span></span>
|<span data-ttu-id="63346-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="63346-121">Header</span></span>|<span data-ttu-id="63346-122">Значение</span><span class="sxs-lookup"><span data-stu-id="63346-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63346-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63346-123">Authorization</span></span>|<span data-ttu-id="63346-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63346-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63346-125">Accept</span><span class="sxs-lookup"><span data-stu-id="63346-125">Accept</span></span>|<span data-ttu-id="63346-126">application/json</span><span class="sxs-lookup"><span data-stu-id="63346-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63346-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="63346-127">Request body</span></span>
<span data-ttu-id="63346-128">В теле запроса добавьте представление объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="63346-128">In the request body, supply a JSON representation for the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

<span data-ttu-id="63346-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="63346-129">The following table shows the properties that are required when you create the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>

|<span data-ttu-id="63346-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="63346-130">Property</span></span>|<span data-ttu-id="63346-131">Тип</span><span class="sxs-lookup"><span data-stu-id="63346-131">Type</span></span>|<span data-ttu-id="63346-132">Описание</span><span class="sxs-lookup"><span data-stu-id="63346-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63346-133">id</span><span class="sxs-lookup"><span data-stu-id="63346-133">id</span></span>|<span data-ttu-id="63346-134">Строка</span><span class="sxs-lookup"><span data-stu-id="63346-134">String</span></span>|<span data-ttu-id="63346-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="63346-135">Key of the entity.</span></span>|
|<span data-ttu-id="63346-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="63346-136">lastModifiedDateTime</span></span>|<span data-ttu-id="63346-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63346-137">DateTimeOffset</span></span>|<span data-ttu-id="63346-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="63346-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="63346-139">displayName</span><span class="sxs-lookup"><span data-stu-id="63346-139">displayName</span></span>|<span data-ttu-id="63346-140">Строка</span><span class="sxs-lookup"><span data-stu-id="63346-140">String</span></span>|<span data-ttu-id="63346-141">Отображаемое имя для шаблона сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="63346-141">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="63346-142">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="63346-142">defaultLocale</span></span>|<span data-ttu-id="63346-143">String</span><span class="sxs-lookup"><span data-stu-id="63346-143">String</span></span>|<span data-ttu-id="63346-144">Языковой стандарт по умолчанию, который используется, если запрошенный языковой стандарт недоступен.</span><span class="sxs-lookup"><span data-stu-id="63346-144">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="63346-145">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="63346-145">brandingOptions</span></span>|[<span data-ttu-id="63346-146">нотификатионтемплатебрандингоптионс</span><span class="sxs-lookup"><span data-stu-id="63346-146">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="63346-147">Параметры фирменной символики шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="63346-147">The Message Template Branding Options.</span></span> <span data-ttu-id="63346-148">Фирменная символика определяется в консоли администрирования Intune.</span><span class="sxs-lookup"><span data-stu-id="63346-148">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="63346-149">Возможные значения: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`, `includeCompanyPortalLink`.</span><span class="sxs-lookup"><span data-stu-id="63346-149">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`, `includeCompanyPortalLink`.</span></span>|
|<span data-ttu-id="63346-150">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="63346-150">roleScopeTagIds</span></span>|<span data-ttu-id="63346-151">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="63346-151">String collection</span></span>|<span data-ttu-id="63346-152">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="63346-152">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="63346-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="63346-153">Response</span></span>
<span data-ttu-id="63346-154">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="63346-154">If successful, this method returns a `200 OK` response code and an updated [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63346-155">Пример</span><span class="sxs-lookup"><span data-stu-id="63346-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="63346-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="63346-156">Request</span></span>
<span data-ttu-id="63346-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63346-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
Content-type: application/json
Content-length: 259

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="63346-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="63346-158">Response</span></span>
<span data-ttu-id="63346-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="63346-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 372

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "e1db399b-399b-e1db-9b39-dbe19b39dbe1",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```






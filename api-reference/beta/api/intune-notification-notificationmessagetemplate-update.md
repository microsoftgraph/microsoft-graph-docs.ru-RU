---
title: Обновление объекта notificationMessageTemplate
description: Обновление свойств объекта notificationMessageTemplate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d5b45f01e8a66d11530b4267b806b1ccd8cd2a0b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152812"
---
# <a name="update-notificationmessagetemplate"></a><span data-ttu-id="d7192-103">Обновление объекта notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="d7192-103">Update notificationMessageTemplate</span></span>

<span data-ttu-id="d7192-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7192-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d7192-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7192-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7192-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d7192-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7192-107">Обновление свойств объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="d7192-107">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7192-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d7192-108">Prerequisites</span></span>
<span data-ttu-id="d7192-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7192-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7192-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7192-111">Permission type</span></span>|<span data-ttu-id="d7192-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7192-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7192-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7192-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d7192-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7192-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d7192-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7192-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7192-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7192-116">Not supported.</span></span>|
|<span data-ttu-id="d7192-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d7192-117">Application</span></span>|<span data-ttu-id="d7192-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7192-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7192-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7192-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="d7192-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d7192-120">Request headers</span></span>
|<span data-ttu-id="d7192-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d7192-121">Header</span></span>|<span data-ttu-id="d7192-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d7192-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7192-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7192-123">Authorization</span></span>|<span data-ttu-id="d7192-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7192-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7192-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d7192-125">Accept</span></span>|<span data-ttu-id="d7192-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d7192-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7192-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7192-127">Request body</span></span>
<span data-ttu-id="d7192-128">В теле запроса добавьте представление объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7192-128">In the request body, supply a JSON representation for the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

<span data-ttu-id="d7192-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="d7192-129">The following table shows the properties that are required when you create the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>

|<span data-ttu-id="d7192-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7192-130">Property</span></span>|<span data-ttu-id="d7192-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d7192-131">Type</span></span>|<span data-ttu-id="d7192-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d7192-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7192-133">id</span><span class="sxs-lookup"><span data-stu-id="d7192-133">id</span></span>|<span data-ttu-id="d7192-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d7192-134">String</span></span>|<span data-ttu-id="d7192-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d7192-135">Key of the entity.</span></span>|
|<span data-ttu-id="d7192-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d7192-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d7192-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7192-137">DateTimeOffset</span></span>|<span data-ttu-id="d7192-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d7192-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="d7192-139">displayName</span><span class="sxs-lookup"><span data-stu-id="d7192-139">displayName</span></span>|<span data-ttu-id="d7192-140">Строка</span><span class="sxs-lookup"><span data-stu-id="d7192-140">String</span></span>|<span data-ttu-id="d7192-141">Отображаемое имя для шаблона сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="d7192-141">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="d7192-142">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="d7192-142">defaultLocale</span></span>|<span data-ttu-id="d7192-143">String</span><span class="sxs-lookup"><span data-stu-id="d7192-143">String</span></span>|<span data-ttu-id="d7192-144">Языковой стандарт по умолчанию, который используется, если запрошенный языковой стандарт недоступен.</span><span class="sxs-lookup"><span data-stu-id="d7192-144">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="d7192-145">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="d7192-145">brandingOptions</span></span>|[<span data-ttu-id="d7192-146">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="d7192-146">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="d7192-147">Параметры фирменной символики шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="d7192-147">The Message Template Branding Options.</span></span> <span data-ttu-id="d7192-148">Фирменная символика определяется в консоли администрирования Intune.</span><span class="sxs-lookup"><span data-stu-id="d7192-148">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="d7192-149">Возможные значения: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`, `includeCompanyPortalLink`.</span><span class="sxs-lookup"><span data-stu-id="d7192-149">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`, `includeCompanyPortalLink`.</span></span>|
|<span data-ttu-id="d7192-150">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d7192-150">roleScopeTagIds</span></span>|<span data-ttu-id="d7192-151">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d7192-151">String collection</span></span>|<span data-ttu-id="d7192-152">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="d7192-152">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="d7192-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7192-153">Response</span></span>
<span data-ttu-id="d7192-154">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d7192-154">If successful, this method returns a `200 OK` response code and an updated [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7192-155">Пример</span><span class="sxs-lookup"><span data-stu-id="d7192-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7192-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7192-156">Request</span></span>
<span data-ttu-id="d7192-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7192-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d7192-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7192-158">Response</span></span>
<span data-ttu-id="d7192-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d7192-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





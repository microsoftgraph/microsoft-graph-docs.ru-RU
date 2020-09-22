---
title: Создание объекта notificationMessageTemplate
description: Создание объекта notificationMessageTemplate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b6ef2b42c948f405bda23c89601c24c661b75f6d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055010"
---
# <a name="create-notificationmessagetemplate"></a><span data-ttu-id="82d45-103">Создание объекта notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="82d45-103">Create notificationMessageTemplate</span></span>

<span data-ttu-id="82d45-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82d45-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="82d45-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="82d45-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82d45-106">Создание объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="82d45-106">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82d45-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="82d45-107">Prerequisites</span></span>
<span data-ttu-id="82d45-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82d45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82d45-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82d45-110">Permission type</span></span>|<span data-ttu-id="82d45-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="82d45-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82d45-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82d45-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82d45-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82d45-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="82d45-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82d45-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82d45-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82d45-115">Not supported.</span></span>|
|<span data-ttu-id="82d45-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82d45-116">Application</span></span>|<span data-ttu-id="82d45-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82d45-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82d45-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82d45-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="82d45-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="82d45-119">Request headers</span></span>
|<span data-ttu-id="82d45-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82d45-120">Header</span></span>|<span data-ttu-id="82d45-121">Значение</span><span class="sxs-lookup"><span data-stu-id="82d45-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82d45-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="82d45-122">Authorization</span></span>|<span data-ttu-id="82d45-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82d45-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82d45-124">Accept</span><span class="sxs-lookup"><span data-stu-id="82d45-124">Accept</span></span>|<span data-ttu-id="82d45-125">application/json</span><span class="sxs-lookup"><span data-stu-id="82d45-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82d45-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="82d45-126">Request body</span></span>
<span data-ttu-id="82d45-127">В теле запроса добавьте представление объекта notificationMessageTemplate в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82d45-127">In the request body, supply a JSON representation for the notificationMessageTemplate object.</span></span>

<span data-ttu-id="82d45-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта notificationMessageTemplate.</span><span class="sxs-lookup"><span data-stu-id="82d45-128">The following table shows the properties that are required when you create the notificationMessageTemplate.</span></span>

|<span data-ttu-id="82d45-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="82d45-129">Property</span></span>|<span data-ttu-id="82d45-130">Тип</span><span class="sxs-lookup"><span data-stu-id="82d45-130">Type</span></span>|<span data-ttu-id="82d45-131">Описание</span><span class="sxs-lookup"><span data-stu-id="82d45-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82d45-132">id</span><span class="sxs-lookup"><span data-stu-id="82d45-132">id</span></span>|<span data-ttu-id="82d45-133">String</span><span class="sxs-lookup"><span data-stu-id="82d45-133">String</span></span>|<span data-ttu-id="82d45-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="82d45-134">Key of the entity.</span></span>|
|<span data-ttu-id="82d45-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="82d45-135">lastModifiedDateTime</span></span>|<span data-ttu-id="82d45-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82d45-136">DateTimeOffset</span></span>|<span data-ttu-id="82d45-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="82d45-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="82d45-138">displayName</span><span class="sxs-lookup"><span data-stu-id="82d45-138">displayName</span></span>|<span data-ttu-id="82d45-139">String</span><span class="sxs-lookup"><span data-stu-id="82d45-139">String</span></span>|<span data-ttu-id="82d45-140">Отображаемое имя для шаблона сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="82d45-140">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="82d45-141">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="82d45-141">defaultLocale</span></span>|<span data-ttu-id="82d45-142">String</span><span class="sxs-lookup"><span data-stu-id="82d45-142">String</span></span>|<span data-ttu-id="82d45-143">Языковой стандарт по умолчанию, который используется, если запрошенный языковой стандарт недоступен.</span><span class="sxs-lookup"><span data-stu-id="82d45-143">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="82d45-144">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="82d45-144">brandingOptions</span></span>|[<span data-ttu-id="82d45-145">нотификатионтемплатебрандингоптионс</span><span class="sxs-lookup"><span data-stu-id="82d45-145">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="82d45-146">Параметры фирменной символики шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="82d45-146">The Message Template Branding Options.</span></span> <span data-ttu-id="82d45-147">Фирменная символика определяется в консоли администрирования Intune.</span><span class="sxs-lookup"><span data-stu-id="82d45-147">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="82d45-148">Возможные значения: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="82d45-148">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|



## <a name="response"></a><span data-ttu-id="82d45-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="82d45-149">Response</span></span>
<span data-ttu-id="82d45-150">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="82d45-150">If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82d45-151">Пример</span><span class="sxs-lookup"><span data-stu-id="82d45-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="82d45-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="82d45-152">Request</span></span>
<span data-ttu-id="82d45-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82d45-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates
Content-type: application/json
Content-length: 197

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo"
}
```

### <a name="response"></a><span data-ttu-id="82d45-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="82d45-154">Response</span></span>
<span data-ttu-id="82d45-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82d45-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 310

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "e1db399b-399b-e1db-9b39-dbe19b39dbe1",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo"
}
```










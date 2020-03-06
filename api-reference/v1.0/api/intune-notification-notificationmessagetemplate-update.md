---
title: Обновление объекта notificationMessageTemplate
description: Обновление свойств объекта notificationMessageTemplate.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1e445f53b745a7341dbebdbe3b6479960f47401d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512729"
---
# <a name="update-notificationmessagetemplate"></a><span data-ttu-id="b6f18-103">Обновление объекта notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="b6f18-103">Update notificationMessageTemplate</span></span>

<span data-ttu-id="b6f18-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6f18-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b6f18-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b6f18-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6f18-106">Обновление свойств объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="b6f18-106">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6f18-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b6f18-107">Prerequisites</span></span>
<span data-ttu-id="b6f18-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6f18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6f18-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6f18-110">Permission type</span></span>|<span data-ttu-id="b6f18-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6f18-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6f18-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6f18-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b6f18-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6f18-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b6f18-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6f18-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6f18-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6f18-115">Not supported.</span></span>|
|<span data-ttu-id="b6f18-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6f18-116">Application</span></span>|<span data-ttu-id="b6f18-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6f18-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6f18-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6f18-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="b6f18-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b6f18-119">Request headers</span></span>
|<span data-ttu-id="b6f18-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b6f18-120">Header</span></span>|<span data-ttu-id="b6f18-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b6f18-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6f18-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6f18-122">Authorization</span></span>|<span data-ttu-id="b6f18-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6f18-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6f18-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b6f18-124">Accept</span></span>|<span data-ttu-id="b6f18-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b6f18-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6f18-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b6f18-126">Request body</span></span>
<span data-ttu-id="b6f18-127">В теле запроса добавьте представление объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6f18-127">In the request body, supply a JSON representation for the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

<span data-ttu-id="b6f18-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="b6f18-128">The following table shows the properties that are required when you create the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>

|<span data-ttu-id="b6f18-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6f18-129">Property</span></span>|<span data-ttu-id="b6f18-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b6f18-130">Type</span></span>|<span data-ttu-id="b6f18-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b6f18-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6f18-132">id</span><span class="sxs-lookup"><span data-stu-id="b6f18-132">id</span></span>|<span data-ttu-id="b6f18-133">String</span><span class="sxs-lookup"><span data-stu-id="b6f18-133">String</span></span>|<span data-ttu-id="b6f18-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b6f18-134">Key of the entity.</span></span>|
|<span data-ttu-id="b6f18-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6f18-135">lastModifiedDateTime</span></span>|<span data-ttu-id="b6f18-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6f18-136">DateTimeOffset</span></span>|<span data-ttu-id="b6f18-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b6f18-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="b6f18-138">displayName</span><span class="sxs-lookup"><span data-stu-id="b6f18-138">displayName</span></span>|<span data-ttu-id="b6f18-139">Строка</span><span class="sxs-lookup"><span data-stu-id="b6f18-139">String</span></span>|<span data-ttu-id="b6f18-140">Отображаемое имя для шаблона сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="b6f18-140">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="b6f18-141">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="b6f18-141">defaultLocale</span></span>|<span data-ttu-id="b6f18-142">String</span><span class="sxs-lookup"><span data-stu-id="b6f18-142">String</span></span>|<span data-ttu-id="b6f18-143">Языковой стандарт по умолчанию, который используется, если запрошенный языковой стандарт недоступен.</span><span class="sxs-lookup"><span data-stu-id="b6f18-143">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="b6f18-144">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="b6f18-144">brandingOptions</span></span>|[<span data-ttu-id="b6f18-145">нотификатионтемплатебрандингоптионс</span><span class="sxs-lookup"><span data-stu-id="b6f18-145">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="b6f18-146">Параметры фирменной символики шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="b6f18-146">The Message Template Branding Options.</span></span> <span data-ttu-id="b6f18-147">Фирменная символика определяется в консоли администрирования Intune.</span><span class="sxs-lookup"><span data-stu-id="b6f18-147">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="b6f18-148">Возможные значения: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="b6f18-148">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|



## <a name="response"></a><span data-ttu-id="b6f18-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6f18-149">Response</span></span>
<span data-ttu-id="b6f18-150">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b6f18-150">If successful, this method returns a `200 OK` response code and an updated [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6f18-151">Пример</span><span class="sxs-lookup"><span data-stu-id="b6f18-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6f18-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6f18-152">Request</span></span>
<span data-ttu-id="b6f18-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6f18-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
Content-type: application/json
Content-length: 197

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo"
}
```

### <a name="response"></a><span data-ttu-id="b6f18-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6f18-154">Response</span></span>
<span data-ttu-id="b6f18-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b6f18-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





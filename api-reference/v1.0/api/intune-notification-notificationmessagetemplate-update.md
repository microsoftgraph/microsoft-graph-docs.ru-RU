---
title: Обновление объекта notificationMessageTemplate
description: Обновление свойств объекта notificationMessageTemplate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 484e719b089157ddf18a165b50230ed84c644b2f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974768"
---
# <a name="update-notificationmessagetemplate"></a><span data-ttu-id="ee98e-103">Обновление объекта notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="ee98e-103">Update notificationMessageTemplate</span></span>

> <span data-ttu-id="ee98e-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee98e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee98e-105">Обновление свойств объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="ee98e-105">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee98e-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ee98e-106">Prerequisites</span></span>
<span data-ttu-id="ee98e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee98e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee98e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee98e-109">Permission type</span></span>|<span data-ttu-id="ee98e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee98e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee98e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee98e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ee98e-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee98e-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ee98e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee98e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee98e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee98e-114">Not supported.</span></span>|
|<span data-ttu-id="ee98e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee98e-115">Application</span></span>|<span data-ttu-id="ee98e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee98e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee98e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee98e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="ee98e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee98e-118">Request headers</span></span>
|<span data-ttu-id="ee98e-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ee98e-119">Header</span></span>|<span data-ttu-id="ee98e-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ee98e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee98e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee98e-121">Authorization</span></span>|<span data-ttu-id="ee98e-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee98e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee98e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ee98e-123">Accept</span></span>|<span data-ttu-id="ee98e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ee98e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee98e-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ee98e-125">Request body</span></span>
<span data-ttu-id="ee98e-126">В теле запроса добавьте представление объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee98e-126">In the request body, supply a JSON representation for the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

<span data-ttu-id="ee98e-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="ee98e-127">The following table shows the properties that are required when you create the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>

|<span data-ttu-id="ee98e-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee98e-128">Property</span></span>|<span data-ttu-id="ee98e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ee98e-129">Type</span></span>|<span data-ttu-id="ee98e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ee98e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee98e-131">id</span><span class="sxs-lookup"><span data-stu-id="ee98e-131">id</span></span>|<span data-ttu-id="ee98e-132">String</span><span class="sxs-lookup"><span data-stu-id="ee98e-132">String</span></span>|<span data-ttu-id="ee98e-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ee98e-133">Key of the entity.</span></span>|
|<span data-ttu-id="ee98e-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee98e-134">lastModifiedDateTime</span></span>|<span data-ttu-id="ee98e-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee98e-135">DateTimeOffset</span></span>|<span data-ttu-id="ee98e-136">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ee98e-136">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="ee98e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ee98e-137">displayName</span></span>|<span data-ttu-id="ee98e-138">Строка</span><span class="sxs-lookup"><span data-stu-id="ee98e-138">String</span></span>|<span data-ttu-id="ee98e-139">Отображаемое имя для шаблона сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="ee98e-139">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="ee98e-140">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="ee98e-140">defaultLocale</span></span>|<span data-ttu-id="ee98e-141">String</span><span class="sxs-lookup"><span data-stu-id="ee98e-141">String</span></span>|<span data-ttu-id="ee98e-142">Языковой стандарт по умолчанию, который используется, если запрошенный языковой стандарт недоступен.</span><span class="sxs-lookup"><span data-stu-id="ee98e-142">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="ee98e-143">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="ee98e-143">brandingOptions</span></span>|[<span data-ttu-id="ee98e-144">Нотификатионтемплатебрандингоптионс</span><span class="sxs-lookup"><span data-stu-id="ee98e-144">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="ee98e-145">Параметры фирменной символики шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="ee98e-145">The Message Template Branding Options.</span></span> <span data-ttu-id="ee98e-146">Фирменная символика определяется в консоли администрирования Intune.</span><span class="sxs-lookup"><span data-stu-id="ee98e-146">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="ee98e-147">Возможные значения: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="ee98e-147">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|



## <a name="response"></a><span data-ttu-id="ee98e-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee98e-148">Response</span></span>
<span data-ttu-id="ee98e-149">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ee98e-149">If successful, this method returns a `200 OK` response code and an updated [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee98e-150">Пример</span><span class="sxs-lookup"><span data-stu-id="ee98e-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee98e-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee98e-151">Request</span></span>
<span data-ttu-id="ee98e-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee98e-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ee98e-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee98e-153">Response</span></span>
<span data-ttu-id="ee98e-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ee98e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




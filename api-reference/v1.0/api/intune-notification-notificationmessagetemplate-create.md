---
title: Создание объекта notificationMessageTemplate
description: Создание объекта notificationMessageTemplate.
ms.openlocfilehash: 9d1d54e992a51344c3310ccf3d63890cd60c15c5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027988"
---
# <a name="create-notificationmessagetemplate"></a><span data-ttu-id="6ce88-103">Создание объекта notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="6ce88-103">Create notificationMessageTemplate</span></span>

> <span data-ttu-id="6ce88-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6ce88-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ce88-105">Создание объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="6ce88-105">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6ce88-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6ce88-106">Prerequisites</span></span>
<span data-ttu-id="6ce88-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ce88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ce88-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ce88-109">Permission type</span></span>|<span data-ttu-id="6ce88-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ce88-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ce88-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ce88-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6ce88-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ce88-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6ce88-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ce88-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ce88-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ce88-114">Not supported.</span></span>|
|<span data-ttu-id="6ce88-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ce88-115">Application</span></span>|<span data-ttu-id="6ce88-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ce88-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ce88-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ce88-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="6ce88-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ce88-118">Request headers</span></span>
|<span data-ttu-id="6ce88-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6ce88-119">Header</span></span>|<span data-ttu-id="6ce88-120">Значение</span><span class="sxs-lookup"><span data-stu-id="6ce88-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ce88-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ce88-121">Authorization</span></span>|<span data-ttu-id="6ce88-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6ce88-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ce88-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6ce88-123">Accept</span></span>|<span data-ttu-id="6ce88-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6ce88-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ce88-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6ce88-125">Request body</span></span>
<span data-ttu-id="6ce88-126">В теле запроса добавьте представление объекта notificationMessageTemplate в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ce88-126">In the request body, supply a JSON representation for the notificationMessageTemplate object.</span></span>

<span data-ttu-id="6ce88-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта notificationMessageTemplate.</span><span class="sxs-lookup"><span data-stu-id="6ce88-127">The following table shows the properties that are required when you create the notificationMessageTemplate.</span></span>

|<span data-ttu-id="6ce88-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ce88-128">Property</span></span>|<span data-ttu-id="6ce88-129">Тип</span><span class="sxs-lookup"><span data-stu-id="6ce88-129">Type</span></span>|<span data-ttu-id="6ce88-130">Описание</span><span class="sxs-lookup"><span data-stu-id="6ce88-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ce88-131">id</span><span class="sxs-lookup"><span data-stu-id="6ce88-131">id</span></span>|<span data-ttu-id="6ce88-132">String</span><span class="sxs-lookup"><span data-stu-id="6ce88-132">String</span></span>|<span data-ttu-id="6ce88-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6ce88-133">Key of the entity.</span></span>|
|<span data-ttu-id="6ce88-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6ce88-134">lastModifiedDateTime</span></span>|<span data-ttu-id="6ce88-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ce88-135">DateTimeOffset</span></span>|<span data-ttu-id="6ce88-136">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6ce88-136">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="6ce88-137">displayName</span><span class="sxs-lookup"><span data-stu-id="6ce88-137">displayName</span></span>|<span data-ttu-id="6ce88-138">String</span><span class="sxs-lookup"><span data-stu-id="6ce88-138">String</span></span>|<span data-ttu-id="6ce88-139">Отображаемое имя для шаблона сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="6ce88-139">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="6ce88-140">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="6ce88-140">defaultLocale</span></span>|<span data-ttu-id="6ce88-141">String</span><span class="sxs-lookup"><span data-stu-id="6ce88-141">String</span></span>|<span data-ttu-id="6ce88-142">Языковой стандарт по умолчанию, который используется, если запрошенный языковой стандарт недоступен.</span><span class="sxs-lookup"><span data-stu-id="6ce88-142">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="6ce88-143">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="6ce88-143">brandingOptions</span></span>|[<span data-ttu-id="6ce88-144">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="6ce88-144">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="6ce88-145">Параметры фирменной символики шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="6ce88-145">The Message Template Branding Options.</span></span> <span data-ttu-id="6ce88-146">Фирменная символика определяется в консоли администрирования Intune.</span><span class="sxs-lookup"><span data-stu-id="6ce88-146">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="6ce88-147">Возможные значения: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="6ce88-147">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|



## <a name="response"></a><span data-ttu-id="6ce88-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ce88-148">Response</span></span>
<span data-ttu-id="6ce88-149">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6ce88-149">If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ce88-150">Пример</span><span class="sxs-lookup"><span data-stu-id="6ce88-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="6ce88-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ce88-151">Request</span></span>
<span data-ttu-id="6ce88-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ce88-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6ce88-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="6ce88-153">Response</span></span>
<span data-ttu-id="6ce88-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="6ce88-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




---
title: Создание объекта notificationMessageTemplate
description: Создание объекта notificationMessageTemplate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 01880bae6f0a1d929192d18cd79baee546470824
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462644"
---
# <a name="create-notificationmessagetemplate"></a><span data-ttu-id="d8854-103">Создание объекта notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="d8854-103">Create notificationMessageTemplate</span></span>

<span data-ttu-id="d8854-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d8854-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8854-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8854-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8854-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8854-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8854-107">Создание объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="d8854-107">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8854-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d8854-108">Prerequisites</span></span>
<span data-ttu-id="d8854-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8854-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8854-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8854-111">Permission type</span></span>|<span data-ttu-id="d8854-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8854-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8854-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8854-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d8854-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8854-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d8854-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8854-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8854-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8854-116">Not supported.</span></span>|
|<span data-ttu-id="d8854-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8854-117">Application</span></span>|<span data-ttu-id="d8854-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8854-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8854-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8854-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="d8854-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d8854-120">Request headers</span></span>
|<span data-ttu-id="d8854-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d8854-121">Header</span></span>|<span data-ttu-id="d8854-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d8854-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8854-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8854-123">Authorization</span></span>|<span data-ttu-id="d8854-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8854-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8854-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d8854-125">Accept</span></span>|<span data-ttu-id="d8854-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d8854-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8854-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8854-127">Request body</span></span>
<span data-ttu-id="d8854-128">В теле запроса добавьте представление объекта notificationMessageTemplate в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8854-128">In the request body, supply a JSON representation for the notificationMessageTemplate object.</span></span>

<span data-ttu-id="d8854-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта notificationMessageTemplate.</span><span class="sxs-lookup"><span data-stu-id="d8854-129">The following table shows the properties that are required when you create the notificationMessageTemplate.</span></span>

|<span data-ttu-id="d8854-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8854-130">Property</span></span>|<span data-ttu-id="d8854-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d8854-131">Type</span></span>|<span data-ttu-id="d8854-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d8854-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8854-133">id</span><span class="sxs-lookup"><span data-stu-id="d8854-133">id</span></span>|<span data-ttu-id="d8854-134">String</span><span class="sxs-lookup"><span data-stu-id="d8854-134">String</span></span>|<span data-ttu-id="d8854-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d8854-135">Key of the entity.</span></span>|
|<span data-ttu-id="d8854-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8854-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d8854-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8854-137">DateTimeOffset</span></span>|<span data-ttu-id="d8854-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d8854-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="d8854-139">displayName</span><span class="sxs-lookup"><span data-stu-id="d8854-139">displayName</span></span>|<span data-ttu-id="d8854-140">Строка</span><span class="sxs-lookup"><span data-stu-id="d8854-140">String</span></span>|<span data-ttu-id="d8854-141">Отображаемое имя для шаблона сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="d8854-141">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="d8854-142">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="d8854-142">defaultLocale</span></span>|<span data-ttu-id="d8854-143">String</span><span class="sxs-lookup"><span data-stu-id="d8854-143">String</span></span>|<span data-ttu-id="d8854-144">Языковой стандарт по умолчанию, который используется, если запрошенный языковой стандарт недоступен.</span><span class="sxs-lookup"><span data-stu-id="d8854-144">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="d8854-145">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="d8854-145">brandingOptions</span></span>|[<span data-ttu-id="d8854-146">нотификатионтемплатебрандингоптионс</span><span class="sxs-lookup"><span data-stu-id="d8854-146">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="d8854-147">Параметры фирменной символики шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="d8854-147">The Message Template Branding Options.</span></span> <span data-ttu-id="d8854-148">Фирменная символика определяется в консоли администрирования Intune.</span><span class="sxs-lookup"><span data-stu-id="d8854-148">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="d8854-149">Возможные значения: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="d8854-149">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|
|<span data-ttu-id="d8854-150">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d8854-150">roleScopeTagIds</span></span>|<span data-ttu-id="d8854-151">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d8854-151">String collection</span></span>|<span data-ttu-id="d8854-152">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d8854-152">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="d8854-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8854-153">Response</span></span>
<span data-ttu-id="d8854-154">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d8854-154">If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8854-155">Пример</span><span class="sxs-lookup"><span data-stu-id="d8854-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8854-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8854-156">Request</span></span>
<span data-ttu-id="d8854-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8854-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates
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

### <a name="response"></a><span data-ttu-id="d8854-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8854-158">Response</span></span>
<span data-ttu-id="d8854-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d8854-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






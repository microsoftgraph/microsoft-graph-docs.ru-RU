---
title: Создание объекта notificationMessageTemplate
description: Создание объекта notificationMessageTemplate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a0252c4a84d3aad9ce6f42c8442878a969626604
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51125886"
---
# <a name="create-notificationmessagetemplate"></a><span data-ttu-id="4f931-103">Создание объекта notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="4f931-103">Create notificationMessageTemplate</span></span>

<span data-ttu-id="4f931-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f931-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f931-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f931-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f931-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f931-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f931-107">Создание объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="4f931-107">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f931-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4f931-108">Prerequisites</span></span>
<span data-ttu-id="4f931-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f931-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f931-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f931-111">Permission type</span></span>|<span data-ttu-id="4f931-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f931-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f931-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f931-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4f931-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f931-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4f931-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f931-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f931-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f931-116">Not supported.</span></span>|
|<span data-ttu-id="4f931-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4f931-117">Application</span></span>|<span data-ttu-id="4f931-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f931-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f931-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f931-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="4f931-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4f931-120">Request headers</span></span>
|<span data-ttu-id="4f931-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f931-121">Header</span></span>|<span data-ttu-id="4f931-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4f931-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f931-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f931-123">Authorization</span></span>|<span data-ttu-id="4f931-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f931-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f931-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4f931-125">Accept</span></span>|<span data-ttu-id="4f931-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4f931-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f931-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f931-127">Request body</span></span>
<span data-ttu-id="4f931-128">В теле запроса добавьте представление объекта notificationMessageTemplate в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f931-128">In the request body, supply a JSON representation for the notificationMessageTemplate object.</span></span>

<span data-ttu-id="4f931-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта notificationMessageTemplate.</span><span class="sxs-lookup"><span data-stu-id="4f931-129">The following table shows the properties that are required when you create the notificationMessageTemplate.</span></span>

|<span data-ttu-id="4f931-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f931-130">Property</span></span>|<span data-ttu-id="4f931-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4f931-131">Type</span></span>|<span data-ttu-id="4f931-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4f931-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f931-133">id</span><span class="sxs-lookup"><span data-stu-id="4f931-133">id</span></span>|<span data-ttu-id="4f931-134">Строка</span><span class="sxs-lookup"><span data-stu-id="4f931-134">String</span></span>|<span data-ttu-id="4f931-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4f931-135">Key of the entity.</span></span>|
|<span data-ttu-id="4f931-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4f931-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4f931-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f931-137">DateTimeOffset</span></span>|<span data-ttu-id="4f931-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4f931-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="4f931-139">displayName</span><span class="sxs-lookup"><span data-stu-id="4f931-139">displayName</span></span>|<span data-ttu-id="4f931-140">Строка</span><span class="sxs-lookup"><span data-stu-id="4f931-140">String</span></span>|<span data-ttu-id="4f931-141">Отображаемое имя для шаблона сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="4f931-141">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="4f931-142">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="4f931-142">defaultLocale</span></span>|<span data-ttu-id="4f931-143">String</span><span class="sxs-lookup"><span data-stu-id="4f931-143">String</span></span>|<span data-ttu-id="4f931-144">Языковой стандарт по умолчанию, который используется, если запрошенный языковой стандарт недоступен.</span><span class="sxs-lookup"><span data-stu-id="4f931-144">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="4f931-145">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="4f931-145">brandingOptions</span></span>|[<span data-ttu-id="4f931-146">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="4f931-146">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="4f931-147">Параметры фирменной символики шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="4f931-147">The Message Template Branding Options.</span></span> <span data-ttu-id="4f931-148">Фирменная символика определяется в консоли администрирования Intune.</span><span class="sxs-lookup"><span data-stu-id="4f931-148">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="4f931-149">Возможные значения: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`, `includeCompanyPortalLink`.</span><span class="sxs-lookup"><span data-stu-id="4f931-149">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`, `includeCompanyPortalLink`.</span></span>|
|<span data-ttu-id="4f931-150">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4f931-150">roleScopeTagIds</span></span>|<span data-ttu-id="4f931-151">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4f931-151">String collection</span></span>|<span data-ttu-id="4f931-152">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="4f931-152">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="4f931-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f931-153">Response</span></span>
<span data-ttu-id="4f931-154">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4f931-154">If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f931-155">Пример</span><span class="sxs-lookup"><span data-stu-id="4f931-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f931-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f931-156">Request</span></span>
<span data-ttu-id="4f931-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f931-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4f931-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f931-158">Response</span></span>
<span data-ttu-id="4f931-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f931-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





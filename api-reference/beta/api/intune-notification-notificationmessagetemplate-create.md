---
title: Создание объекта notificationMessageTemplate
description: Создание объекта notificationMessageTemplate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3a4634f40c9c04b9923f2389bb07212ed5af2170
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33900511"
---
# <a name="create-notificationmessagetemplate"></a><span data-ttu-id="0ee74-103">Создание объекта notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="0ee74-103">Create notificationMessageTemplate</span></span>

> <span data-ttu-id="0ee74-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ee74-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ee74-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0ee74-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ee74-106">Создание объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="0ee74-106">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ee74-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0ee74-107">Prerequisites</span></span>
<span data-ttu-id="0ee74-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ee74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ee74-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ee74-110">Permission type</span></span>|<span data-ttu-id="0ee74-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ee74-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ee74-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ee74-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0ee74-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ee74-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0ee74-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ee74-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ee74-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ee74-115">Not supported.</span></span>|
|<span data-ttu-id="0ee74-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ee74-116">Application</span></span>|<span data-ttu-id="0ee74-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ee74-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ee74-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ee74-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="0ee74-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ee74-119">Request headers</span></span>
|<span data-ttu-id="0ee74-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0ee74-120">Header</span></span>|<span data-ttu-id="0ee74-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0ee74-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ee74-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ee74-122">Authorization</span></span>|<span data-ttu-id="0ee74-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ee74-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ee74-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0ee74-124">Accept</span></span>|<span data-ttu-id="0ee74-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0ee74-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ee74-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ee74-126">Request body</span></span>
<span data-ttu-id="0ee74-127">В теле запроса добавьте представление объекта notificationMessageTemplate в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ee74-127">In the request body, supply a JSON representation for the notificationMessageTemplate object.</span></span>

<span data-ttu-id="0ee74-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта notificationMessageTemplate.</span><span class="sxs-lookup"><span data-stu-id="0ee74-128">The following table shows the properties that are required when you create the notificationMessageTemplate.</span></span>

|<span data-ttu-id="0ee74-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ee74-129">Property</span></span>|<span data-ttu-id="0ee74-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0ee74-130">Type</span></span>|<span data-ttu-id="0ee74-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0ee74-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ee74-132">id</span><span class="sxs-lookup"><span data-stu-id="0ee74-132">id</span></span>|<span data-ttu-id="0ee74-133">String</span><span class="sxs-lookup"><span data-stu-id="0ee74-133">String</span></span>|<span data-ttu-id="0ee74-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0ee74-134">Key of the entity.</span></span>|
|<span data-ttu-id="0ee74-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ee74-135">lastModifiedDateTime</span></span>|<span data-ttu-id="0ee74-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ee74-136">DateTimeOffset</span></span>|<span data-ttu-id="0ee74-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="0ee74-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="0ee74-138">displayName</span><span class="sxs-lookup"><span data-stu-id="0ee74-138">displayName</span></span>|<span data-ttu-id="0ee74-139">Строка</span><span class="sxs-lookup"><span data-stu-id="0ee74-139">String</span></span>|<span data-ttu-id="0ee74-140">Отображаемое имя для шаблона сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="0ee74-140">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="0ee74-141">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="0ee74-141">defaultLocale</span></span>|<span data-ttu-id="0ee74-142">String</span><span class="sxs-lookup"><span data-stu-id="0ee74-142">String</span></span>|<span data-ttu-id="0ee74-143">Языковой стандарт по умолчанию, который используется, если запрошенный языковой стандарт недоступен.</span><span class="sxs-lookup"><span data-stu-id="0ee74-143">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="0ee74-144">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="0ee74-144">brandingOptions</span></span>|[<span data-ttu-id="0ee74-145">Нотификатионтемплатебрандингоптионс</span><span class="sxs-lookup"><span data-stu-id="0ee74-145">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="0ee74-146">Параметры фирменной символики шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="0ee74-146">The Message Template Branding Options.</span></span> <span data-ttu-id="0ee74-147">Фирменная символика определяется в консоли администрирования Intune.</span><span class="sxs-lookup"><span data-stu-id="0ee74-147">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="0ee74-148">Возможные значения: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="0ee74-148">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|
|<span data-ttu-id="0ee74-149">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0ee74-149">roleScopeTagIds</span></span>|<span data-ttu-id="0ee74-150">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0ee74-150">String collection</span></span>|<span data-ttu-id="0ee74-151">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="0ee74-151">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="0ee74-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ee74-152">Response</span></span>
<span data-ttu-id="0ee74-153">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0ee74-153">If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ee74-154">Пример</span><span class="sxs-lookup"><span data-stu-id="0ee74-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ee74-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ee74-155">Request</span></span>
<span data-ttu-id="0ee74-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ee74-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0ee74-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ee74-157">Response</span></span>
<span data-ttu-id="0ee74-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0ee74-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





---
title: Создание объекта notificationMessageTemplate
description: Создание объекта notificationMessageTemplate.
ms.openlocfilehash: 013acd831979fdbb22eb67be66552b2d21d590b6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082862"
---
# <a name="create-notificationmessagetemplate"></a><span data-ttu-id="2ca92-103">Создание объекта notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="2ca92-103">Create notificationMessageTemplate</span></span>

> <span data-ttu-id="2ca92-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2ca92-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2ca92-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ca92-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2ca92-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2ca92-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2ca92-107">Создание объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="2ca92-107">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2ca92-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2ca92-108">Prerequisites</span></span>
<span data-ttu-id="2ca92-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ca92-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ca92-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ca92-111">Permission type</span></span>|<span data-ttu-id="2ca92-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ca92-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ca92-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ca92-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2ca92-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ca92-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2ca92-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ca92-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ca92-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ca92-116">Not supported.</span></span>|
|<span data-ttu-id="2ca92-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ca92-117">Application</span></span>|<span data-ttu-id="2ca92-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ca92-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ca92-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ca92-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="2ca92-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ca92-120">Request headers</span></span>
|<span data-ttu-id="2ca92-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2ca92-121">Header</span></span>|<span data-ttu-id="2ca92-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2ca92-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ca92-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ca92-123">Authorization</span></span>|<span data-ttu-id="2ca92-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2ca92-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ca92-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2ca92-125">Accept</span></span>|<span data-ttu-id="2ca92-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2ca92-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ca92-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2ca92-127">Request body</span></span>
<span data-ttu-id="2ca92-128">В теле запроса добавьте представление объекта notificationMessageTemplate в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ca92-128">In the request body, supply a JSON representation for the notificationMessageTemplate object.</span></span>

<span data-ttu-id="2ca92-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта notificationMessageTemplate.</span><span class="sxs-lookup"><span data-stu-id="2ca92-129">The following table shows the properties that are required when you create the notificationMessageTemplate.</span></span>

|<span data-ttu-id="2ca92-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ca92-130">Property</span></span>|<span data-ttu-id="2ca92-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2ca92-131">Type</span></span>|<span data-ttu-id="2ca92-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2ca92-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ca92-133">id</span><span class="sxs-lookup"><span data-stu-id="2ca92-133">id</span></span>|<span data-ttu-id="2ca92-134">String</span><span class="sxs-lookup"><span data-stu-id="2ca92-134">String</span></span>|<span data-ttu-id="2ca92-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2ca92-135">Key of the entity.</span></span>|
|<span data-ttu-id="2ca92-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ca92-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2ca92-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ca92-137">DateTimeOffset</span></span>|<span data-ttu-id="2ca92-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2ca92-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="2ca92-139">displayName</span><span class="sxs-lookup"><span data-stu-id="2ca92-139">displayName</span></span>|<span data-ttu-id="2ca92-140">String</span><span class="sxs-lookup"><span data-stu-id="2ca92-140">String</span></span>|<span data-ttu-id="2ca92-141">Отображаемое имя для шаблона сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="2ca92-141">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="2ca92-142">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="2ca92-142">defaultLocale</span></span>|<span data-ttu-id="2ca92-143">String</span><span class="sxs-lookup"><span data-stu-id="2ca92-143">String</span></span>|<span data-ttu-id="2ca92-144">Языковой стандарт по умолчанию, который используется, если запрошенный языковой стандарт недоступен.</span><span class="sxs-lookup"><span data-stu-id="2ca92-144">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="2ca92-145">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="2ca92-145">brandingOptions</span></span>|[<span data-ttu-id="2ca92-146">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="2ca92-146">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="2ca92-147">Параметры фирменной символики шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="2ca92-147">The Message Template Branding Options.</span></span> <span data-ttu-id="2ca92-148">Фирменная символика определяется в консоли администрирования Intune.</span><span class="sxs-lookup"><span data-stu-id="2ca92-148">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="2ca92-149">Возможные значения: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="2ca92-149">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|
|<span data-ttu-id="2ca92-150">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2ca92-150">roleScopeTagIds</span></span>|<span data-ttu-id="2ca92-151">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2ca92-151">String collection</span></span>|<span data-ttu-id="2ca92-152">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="2ca92-152">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="2ca92-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ca92-153">Response</span></span>
<span data-ttu-id="2ca92-154">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2ca92-154">If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ca92-155">Пример</span><span class="sxs-lookup"><span data-stu-id="2ca92-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="2ca92-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ca92-156">Request</span></span>
<span data-ttu-id="2ca92-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ca92-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates
Content-type: application/json
Content-length: 323

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="2ca92-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="2ca92-158">Response</span></span>
<span data-ttu-id="2ca92-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="2ca92-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






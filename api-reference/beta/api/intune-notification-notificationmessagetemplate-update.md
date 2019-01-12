---
title: Обновление объекта notificationMessageTemplate
description: Обновление свойств объекта notificationMessageTemplate.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b417ec424ad6a13c576cdfc1cbf62e442b3dfda2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27992002"
---
# <a name="update-notificationmessagetemplate"></a><span data-ttu-id="dc70a-103">Обновление объекта notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="dc70a-103">Update notificationMessageTemplate</span></span>

> <span data-ttu-id="dc70a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dc70a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc70a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc70a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dc70a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dc70a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc70a-107">Обновление свойств объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="dc70a-107">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dc70a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="dc70a-108">Prerequisites</span></span>
<span data-ttu-id="dc70a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc70a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc70a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc70a-111">Permission type</span></span>|<span data-ttu-id="dc70a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc70a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc70a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc70a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dc70a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc70a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="dc70a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc70a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc70a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc70a-116">Not supported.</span></span>|
|<span data-ttu-id="dc70a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc70a-117">Application</span></span>|<span data-ttu-id="dc70a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc70a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc70a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc70a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="dc70a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc70a-120">Request headers</span></span>
|<span data-ttu-id="dc70a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dc70a-121">Header</span></span>|<span data-ttu-id="dc70a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dc70a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc70a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc70a-123">Authorization</span></span>|<span data-ttu-id="dc70a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="dc70a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc70a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dc70a-125">Accept</span></span>|<span data-ttu-id="dc70a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dc70a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc70a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dc70a-127">Request body</span></span>
<span data-ttu-id="dc70a-128">В теле запроса добавьте представление объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dc70a-128">In the request body, supply a JSON representation for the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

<span data-ttu-id="dc70a-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="dc70a-129">The following table shows the properties that are required when you create the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>

|<span data-ttu-id="dc70a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dc70a-130">Property</span></span>|<span data-ttu-id="dc70a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dc70a-131">Type</span></span>|<span data-ttu-id="dc70a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dc70a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc70a-133">id</span><span class="sxs-lookup"><span data-stu-id="dc70a-133">id</span></span>|<span data-ttu-id="dc70a-134">String</span><span class="sxs-lookup"><span data-stu-id="dc70a-134">String</span></span>|<span data-ttu-id="dc70a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dc70a-135">Key of the entity.</span></span>|
|<span data-ttu-id="dc70a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dc70a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="dc70a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc70a-137">DateTimeOffset</span></span>|<span data-ttu-id="dc70a-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="dc70a-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="dc70a-139">displayName</span><span class="sxs-lookup"><span data-stu-id="dc70a-139">displayName</span></span>|<span data-ttu-id="dc70a-140">String</span><span class="sxs-lookup"><span data-stu-id="dc70a-140">String</span></span>|<span data-ttu-id="dc70a-141">Отображаемое имя для шаблона сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="dc70a-141">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="dc70a-142">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="dc70a-142">defaultLocale</span></span>|<span data-ttu-id="dc70a-143">String</span><span class="sxs-lookup"><span data-stu-id="dc70a-143">String</span></span>|<span data-ttu-id="dc70a-144">Языковой стандарт по умолчанию, который используется, если запрошенный языковой стандарт недоступен.</span><span class="sxs-lookup"><span data-stu-id="dc70a-144">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="dc70a-145">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="dc70a-145">brandingOptions</span></span>|[<span data-ttu-id="dc70a-146">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="dc70a-146">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="dc70a-147">Параметры фирменной символики шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="dc70a-147">The Message Template Branding Options.</span></span> <span data-ttu-id="dc70a-148">Фирменная символика определяется в консоли администрирования Intune.</span><span class="sxs-lookup"><span data-stu-id="dc70a-148">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="dc70a-149">Возможные значения: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="dc70a-149">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|
|<span data-ttu-id="dc70a-150">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dc70a-150">roleScopeTagIds</span></span>|<span data-ttu-id="dc70a-151">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="dc70a-151">String collection</span></span>|<span data-ttu-id="dc70a-152">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="dc70a-152">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="dc70a-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc70a-153">Response</span></span>
<span data-ttu-id="dc70a-154">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dc70a-154">If successful, this method returns a `200 OK` response code and an updated [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc70a-155">Пример</span><span class="sxs-lookup"><span data-stu-id="dc70a-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="dc70a-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc70a-156">Request</span></span>
<span data-ttu-id="dc70a-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc70a-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
Content-type: application/json
Content-length: 257

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="dc70a-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="dc70a-158">Response</span></span>
<span data-ttu-id="dc70a-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="dc70a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






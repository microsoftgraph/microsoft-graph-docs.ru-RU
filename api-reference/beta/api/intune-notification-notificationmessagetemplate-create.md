---
title: Создание объекта notificationMessageTemplate
description: Создание объекта notificationMessageTemplate.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f16d9e679533e56e59393f967b9b192b74f3607b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419823"
---
# <a name="create-notificationmessagetemplate"></a><span data-ttu-id="af1cd-103">Создание объекта notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="af1cd-103">Create notificationMessageTemplate</span></span>

> <span data-ttu-id="af1cd-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="af1cd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="af1cd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af1cd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="af1cd-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="af1cd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af1cd-107">Создание объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="af1cd-107">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af1cd-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="af1cd-108">Prerequisites</span></span>
<span data-ttu-id="af1cd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="af1cd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="af1cd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af1cd-111">Permission type</span></span>|<span data-ttu-id="af1cd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="af1cd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af1cd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af1cd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="af1cd-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af1cd-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="af1cd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af1cd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af1cd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af1cd-116">Not supported.</span></span>|
|<span data-ttu-id="af1cd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af1cd-117">Application</span></span>|<span data-ttu-id="af1cd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af1cd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af1cd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af1cd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="af1cd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="af1cd-120">Request headers</span></span>
|<span data-ttu-id="af1cd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="af1cd-121">Header</span></span>|<span data-ttu-id="af1cd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="af1cd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af1cd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="af1cd-123">Authorization</span></span>|<span data-ttu-id="af1cd-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="af1cd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af1cd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="af1cd-125">Accept</span></span>|<span data-ttu-id="af1cd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="af1cd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af1cd-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="af1cd-127">Request body</span></span>
<span data-ttu-id="af1cd-128">В теле запроса добавьте представление объекта notificationMessageTemplate в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af1cd-128">In the request body, supply a JSON representation for the notificationMessageTemplate object.</span></span>

<span data-ttu-id="af1cd-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта notificationMessageTemplate.</span><span class="sxs-lookup"><span data-stu-id="af1cd-129">The following table shows the properties that are required when you create the notificationMessageTemplate.</span></span>

|<span data-ttu-id="af1cd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="af1cd-130">Property</span></span>|<span data-ttu-id="af1cd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="af1cd-131">Type</span></span>|<span data-ttu-id="af1cd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="af1cd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af1cd-133">id</span><span class="sxs-lookup"><span data-stu-id="af1cd-133">id</span></span>|<span data-ttu-id="af1cd-134">String</span><span class="sxs-lookup"><span data-stu-id="af1cd-134">String</span></span>|<span data-ttu-id="af1cd-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="af1cd-135">Key of the entity.</span></span>|
|<span data-ttu-id="af1cd-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="af1cd-136">lastModifiedDateTime</span></span>|<span data-ttu-id="af1cd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af1cd-137">DateTimeOffset</span></span>|<span data-ttu-id="af1cd-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="af1cd-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="af1cd-139">displayName</span><span class="sxs-lookup"><span data-stu-id="af1cd-139">displayName</span></span>|<span data-ttu-id="af1cd-140">String</span><span class="sxs-lookup"><span data-stu-id="af1cd-140">String</span></span>|<span data-ttu-id="af1cd-141">Отображаемое имя для шаблона сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="af1cd-141">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="af1cd-142">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="af1cd-142">defaultLocale</span></span>|<span data-ttu-id="af1cd-143">String</span><span class="sxs-lookup"><span data-stu-id="af1cd-143">String</span></span>|<span data-ttu-id="af1cd-144">Языковой стандарт по умолчанию, который используется, если запрошенный языковой стандарт недоступен.</span><span class="sxs-lookup"><span data-stu-id="af1cd-144">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="af1cd-145">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="af1cd-145">brandingOptions</span></span>|[<span data-ttu-id="af1cd-146">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="af1cd-146">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="af1cd-147">Параметры фирменной символики шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="af1cd-147">The Message Template Branding Options.</span></span> <span data-ttu-id="af1cd-148">Фирменная символика определяется в консоли администрирования Intune.</span><span class="sxs-lookup"><span data-stu-id="af1cd-148">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="af1cd-149">Возможные значения: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="af1cd-149">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|
|<span data-ttu-id="af1cd-150">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="af1cd-150">roleScopeTagIds</span></span>|<span data-ttu-id="af1cd-151">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="af1cd-151">String collection</span></span>|<span data-ttu-id="af1cd-152">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="af1cd-152">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="af1cd-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="af1cd-153">Response</span></span>
<span data-ttu-id="af1cd-154">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="af1cd-154">If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af1cd-155">Пример</span><span class="sxs-lookup"><span data-stu-id="af1cd-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="af1cd-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="af1cd-156">Request</span></span>
<span data-ttu-id="af1cd-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af1cd-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="af1cd-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="af1cd-158">Response</span></span>
<span data-ttu-id="af1cd-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="af1cd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





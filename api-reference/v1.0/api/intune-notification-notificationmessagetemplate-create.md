---
title: Создание объекта notificationMessageTemplate
description: Создание объекта notificationMessageTemplate.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6a79dc797bd91ea58ea6997d18d789c0e6c6e297
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250259"
---
# <a name="create-notificationmessagetemplate"></a><span data-ttu-id="53af3-103">Создание объекта notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="53af3-103">Create notificationMessageTemplate</span></span>

> <span data-ttu-id="53af3-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="53af3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53af3-105">Создание объекта [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="53af3-105">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53af3-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="53af3-106">Prerequisites</span></span>
<span data-ttu-id="53af3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="53af3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="53af3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53af3-109">Permission type</span></span>|<span data-ttu-id="53af3-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="53af3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53af3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53af3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="53af3-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53af3-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="53af3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53af3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53af3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53af3-114">Not supported.</span></span>|
|<span data-ttu-id="53af3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53af3-115">Application</span></span>|<span data-ttu-id="53af3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53af3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53af3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53af3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="53af3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53af3-118">Request headers</span></span>
|<span data-ttu-id="53af3-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="53af3-119">Header</span></span>|<span data-ttu-id="53af3-120">Значение</span><span class="sxs-lookup"><span data-stu-id="53af3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53af3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="53af3-121">Authorization</span></span>|<span data-ttu-id="53af3-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="53af3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53af3-123">Accept</span><span class="sxs-lookup"><span data-stu-id="53af3-123">Accept</span></span>|<span data-ttu-id="53af3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="53af3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53af3-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="53af3-125">Request body</span></span>
<span data-ttu-id="53af3-126">В теле запроса добавьте представление объекта notificationMessageTemplate в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53af3-126">In the request body, supply a JSON representation for the notificationMessageTemplate object.</span></span>

<span data-ttu-id="53af3-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта notificationMessageTemplate.</span><span class="sxs-lookup"><span data-stu-id="53af3-127">The following table shows the properties that are required when you create the notificationMessageTemplate.</span></span>

|<span data-ttu-id="53af3-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="53af3-128">Property</span></span>|<span data-ttu-id="53af3-129">Тип</span><span class="sxs-lookup"><span data-stu-id="53af3-129">Type</span></span>|<span data-ttu-id="53af3-130">Описание</span><span class="sxs-lookup"><span data-stu-id="53af3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53af3-131">id</span><span class="sxs-lookup"><span data-stu-id="53af3-131">id</span></span>|<span data-ttu-id="53af3-132">Строка</span><span class="sxs-lookup"><span data-stu-id="53af3-132">String</span></span>|<span data-ttu-id="53af3-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="53af3-133">Key of the entity.</span></span>|
|<span data-ttu-id="53af3-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="53af3-134">lastModifiedDateTime</span></span>|<span data-ttu-id="53af3-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53af3-135">DateTimeOffset</span></span>|<span data-ttu-id="53af3-136">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="53af3-136">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="53af3-137">displayName</span><span class="sxs-lookup"><span data-stu-id="53af3-137">displayName</span></span>|<span data-ttu-id="53af3-138">String</span><span class="sxs-lookup"><span data-stu-id="53af3-138">String</span></span>|<span data-ttu-id="53af3-139">Отображаемое имя для шаблона сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="53af3-139">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="53af3-140">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="53af3-140">defaultLocale</span></span>|<span data-ttu-id="53af3-141">String</span><span class="sxs-lookup"><span data-stu-id="53af3-141">String</span></span>|<span data-ttu-id="53af3-142">Языковой стандарт по умолчанию, который используется, если запрошенный языковой стандарт недоступен.</span><span class="sxs-lookup"><span data-stu-id="53af3-142">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="53af3-143">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="53af3-143">brandingOptions</span></span>|[<span data-ttu-id="53af3-144">Нотификатионтемплатебрандингоптионс</span><span class="sxs-lookup"><span data-stu-id="53af3-144">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="53af3-145">Параметры фирменной символики шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="53af3-145">The Message Template Branding Options.</span></span> <span data-ttu-id="53af3-146">Фирменная символика определяется в консоли администрирования Intune.</span><span class="sxs-lookup"><span data-stu-id="53af3-146">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="53af3-147">Возможные значения: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="53af3-147">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|



## <a name="response"></a><span data-ttu-id="53af3-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="53af3-148">Response</span></span>
<span data-ttu-id="53af3-149">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="53af3-149">If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53af3-150">Пример</span><span class="sxs-lookup"><span data-stu-id="53af3-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="53af3-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="53af3-151">Request</span></span>
<span data-ttu-id="53af3-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53af3-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="53af3-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="53af3-153">Response</span></span>
<span data-ttu-id="53af3-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="53af3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




---
title: Обновление объекта localizedNotificationMessage
description: Обновление свойств объекта localizedNotificationMessage.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3ce594b97678990a8f8b082929235dd9e1406537
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37191209"
---
# <a name="update-localizednotificationmessage"></a><span data-ttu-id="af717-103">Обновление объекта localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="af717-103">Update localizedNotificationMessage</span></span>

> <span data-ttu-id="af717-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af717-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af717-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="af717-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af717-106">Обновление свойств объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="af717-106">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af717-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="af717-107">Prerequisites</span></span>
<span data-ttu-id="af717-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af717-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af717-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af717-110">Permission type</span></span>|<span data-ttu-id="af717-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="af717-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af717-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af717-112">Delegated (work or school account)</span></span>|<span data-ttu-id="af717-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af717-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="af717-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af717-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af717-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af717-115">Not supported.</span></span>|
|<span data-ttu-id="af717-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af717-116">Application</span></span>|<span data-ttu-id="af717-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af717-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="af717-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af717-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="af717-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="af717-119">Request headers</span></span>
|<span data-ttu-id="af717-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="af717-120">Header</span></span>|<span data-ttu-id="af717-121">Значение</span><span class="sxs-lookup"><span data-stu-id="af717-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af717-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="af717-122">Authorization</span></span>|<span data-ttu-id="af717-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af717-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af717-124">Accept</span><span class="sxs-lookup"><span data-stu-id="af717-124">Accept</span></span>|<span data-ttu-id="af717-125">application/json</span><span class="sxs-lookup"><span data-stu-id="af717-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af717-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="af717-126">Request body</span></span>
<span data-ttu-id="af717-127">В теле запроса добавьте представление объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af717-127">In the request body, supply a JSON representation for the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

<span data-ttu-id="af717-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="af717-128">The following table shows the properties that are required when you create the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

|<span data-ttu-id="af717-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="af717-129">Property</span></span>|<span data-ttu-id="af717-130">Тип</span><span class="sxs-lookup"><span data-stu-id="af717-130">Type</span></span>|<span data-ttu-id="af717-131">Описание</span><span class="sxs-lookup"><span data-stu-id="af717-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af717-132">id</span><span class="sxs-lookup"><span data-stu-id="af717-132">id</span></span>|<span data-ttu-id="af717-133">Строка</span><span class="sxs-lookup"><span data-stu-id="af717-133">String</span></span>|<span data-ttu-id="af717-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="af717-134">Key of the entity.</span></span>|
|<span data-ttu-id="af717-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="af717-135">lastModifiedDateTime</span></span>|<span data-ttu-id="af717-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af717-136">DateTimeOffset</span></span>|<span data-ttu-id="af717-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="af717-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="af717-138">locale</span><span class="sxs-lookup"><span data-stu-id="af717-138">locale</span></span>|<span data-ttu-id="af717-139">String.</span><span class="sxs-lookup"><span data-stu-id="af717-139">String</span></span>|<span data-ttu-id="af717-140">Языковой стандарт, для которого предназначено сообщение.</span><span class="sxs-lookup"><span data-stu-id="af717-140">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="af717-141">subject</span><span class="sxs-lookup"><span data-stu-id="af717-141">subject</span></span>|<span data-ttu-id="af717-142">String</span><span class="sxs-lookup"><span data-stu-id="af717-142">String</span></span>|<span data-ttu-id="af717-143">Тема шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="af717-143">The Message Template Subject.</span></span>|
|<span data-ttu-id="af717-144">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="af717-144">messageTemplate</span></span>|<span data-ttu-id="af717-145">String</span><span class="sxs-lookup"><span data-stu-id="af717-145">String</span></span>|<span data-ttu-id="af717-146">Содержимое шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="af717-146">The Message Template content.</span></span>|
|<span data-ttu-id="af717-147">isDefault</span><span class="sxs-lookup"><span data-stu-id="af717-147">isDefault</span></span>|<span data-ttu-id="af717-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="af717-148">Boolean</span></span>|<span data-ttu-id="af717-149">Флаг, указывающий, используется ли этот языковой стандарт в качестве базового языка.</span><span class="sxs-lookup"><span data-stu-id="af717-149">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="af717-150">Можно устанавливать только этот флаг.</span><span class="sxs-lookup"><span data-stu-id="af717-150">This flag can only be set.</span></span> <span data-ttu-id="af717-151">Чтобы снять его, задайте этому свойству значение true для другого локализованного сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="af717-151">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="af717-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="af717-152">Response</span></span>
<span data-ttu-id="af717-153">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="af717-153">If successful, this method returns a `200 OK` response code and an updated [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af717-154">Пример</span><span class="sxs-lookup"><span data-stu-id="af717-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="af717-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="af717-155">Request</span></span>
<span data-ttu-id="af717-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af717-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
Content-type: application/json
Content-length: 200

{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```

### <a name="response"></a><span data-ttu-id="af717-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="af717-157">Response</span></span>
<span data-ttu-id="af717-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="af717-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 313

{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "id": "7a777708-7708-7a77-0877-777a0877777a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```





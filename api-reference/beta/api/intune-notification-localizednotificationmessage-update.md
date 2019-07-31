---
title: Обновление объекта localizedNotificationMessage
description: Обновление свойств объекта localizedNotificationMessage.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b42352c6f0704614c7085d4edc089802b4fe269c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35994336"
---
# <a name="update-localizednotificationmessage"></a><span data-ttu-id="a1317-103">Обновление объекта localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="a1317-103">Update localizedNotificationMessage</span></span>

> <span data-ttu-id="a1317-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1317-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1317-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a1317-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1317-106">Обновление свойств объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="a1317-106">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1317-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a1317-107">Prerequisites</span></span>
<span data-ttu-id="a1317-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1317-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1317-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1317-110">Permission type</span></span>|<span data-ttu-id="a1317-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1317-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1317-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1317-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1317-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1317-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a1317-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1317-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1317-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1317-115">Not supported.</span></span>|
|<span data-ttu-id="a1317-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1317-116">Application</span></span>|<span data-ttu-id="a1317-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1317-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1317-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1317-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="a1317-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1317-119">Request headers</span></span>
|<span data-ttu-id="a1317-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a1317-120">Header</span></span>|<span data-ttu-id="a1317-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a1317-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1317-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a1317-122">Authorization</span></span>|<span data-ttu-id="a1317-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1317-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1317-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a1317-124">Accept</span></span>|<span data-ttu-id="a1317-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a1317-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1317-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a1317-126">Request body</span></span>
<span data-ttu-id="a1317-127">В теле запроса добавьте представление объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a1317-127">In the request body, supply a JSON representation for the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

<span data-ttu-id="a1317-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="a1317-128">The following table shows the properties that are required when you create the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

|<span data-ttu-id="a1317-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a1317-129">Property</span></span>|<span data-ttu-id="a1317-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a1317-130">Type</span></span>|<span data-ttu-id="a1317-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a1317-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1317-132">id</span><span class="sxs-lookup"><span data-stu-id="a1317-132">id</span></span>|<span data-ttu-id="a1317-133">Строка</span><span class="sxs-lookup"><span data-stu-id="a1317-133">String</span></span>|<span data-ttu-id="a1317-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a1317-134">Key of the entity.</span></span>|
|<span data-ttu-id="a1317-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1317-135">lastModifiedDateTime</span></span>|<span data-ttu-id="a1317-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1317-136">DateTimeOffset</span></span>|<span data-ttu-id="a1317-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a1317-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="a1317-138">locale</span><span class="sxs-lookup"><span data-stu-id="a1317-138">locale</span></span>|<span data-ttu-id="a1317-139">String</span><span class="sxs-lookup"><span data-stu-id="a1317-139">String</span></span>|<span data-ttu-id="a1317-140">Языковой стандарт, для которого предназначено сообщение.</span><span class="sxs-lookup"><span data-stu-id="a1317-140">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="a1317-141">subject</span><span class="sxs-lookup"><span data-stu-id="a1317-141">subject</span></span>|<span data-ttu-id="a1317-142">String</span><span class="sxs-lookup"><span data-stu-id="a1317-142">String</span></span>|<span data-ttu-id="a1317-143">Тема шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="a1317-143">The Message Template Subject.</span></span>|
|<span data-ttu-id="a1317-144">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="a1317-144">messageTemplate</span></span>|<span data-ttu-id="a1317-145">String</span><span class="sxs-lookup"><span data-stu-id="a1317-145">String</span></span>|<span data-ttu-id="a1317-146">Содержимое шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="a1317-146">The Message Template content.</span></span>|
|<span data-ttu-id="a1317-147">isDefault</span><span class="sxs-lookup"><span data-stu-id="a1317-147">isDefault</span></span>|<span data-ttu-id="a1317-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1317-148">Boolean</span></span>|<span data-ttu-id="a1317-149">Флаг, указывающий, используется ли этот языковой стандарт в качестве базового языка.</span><span class="sxs-lookup"><span data-stu-id="a1317-149">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="a1317-150">Можно устанавливать только этот флаг.</span><span class="sxs-lookup"><span data-stu-id="a1317-150">This flag can only be set.</span></span> <span data-ttu-id="a1317-151">Чтобы снять его, задайте этому свойству значение true для другого локализованного сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="a1317-151">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="a1317-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1317-152">Response</span></span>
<span data-ttu-id="a1317-153">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a1317-153">If successful, this method returns a `200 OK` response code and an updated [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1317-154">Пример</span><span class="sxs-lookup"><span data-stu-id="a1317-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1317-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1317-155">Request</span></span>
<span data-ttu-id="a1317-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1317-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a1317-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1317-157">Response</span></span>
<span data-ttu-id="a1317-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a1317-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






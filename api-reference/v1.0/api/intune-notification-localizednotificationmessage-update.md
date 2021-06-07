---
title: Обновление объекта localizedNotificationMessage
description: Обновление свойств объекта localizedNotificationMessage.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 038772c30fa6b4f732b08f8a7895cb9a10ca92f9
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754883"
---
# <a name="update-localizednotificationmessage"></a><span data-ttu-id="e9732-103">Обновление объекта localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="e9732-103">Update localizedNotificationMessage</span></span>

<span data-ttu-id="e9732-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9732-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e9732-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e9732-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9732-106">Обновление свойств объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="e9732-106">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9732-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e9732-107">Prerequisites</span></span>
<span data-ttu-id="e9732-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9732-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9732-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9732-110">Permission type</span></span>|<span data-ttu-id="e9732-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9732-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9732-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9732-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e9732-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9732-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e9732-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9732-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9732-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9732-115">Not supported.</span></span>|
|<span data-ttu-id="e9732-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="e9732-116">Application</span></span>|<span data-ttu-id="e9732-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9732-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9732-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9732-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="e9732-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e9732-119">Request headers</span></span>
|<span data-ttu-id="e9732-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e9732-120">Header</span></span>|<span data-ttu-id="e9732-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e9732-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9732-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9732-122">Authorization</span></span>|<span data-ttu-id="e9732-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9732-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9732-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e9732-124">Accept</span></span>|<span data-ttu-id="e9732-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e9732-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9732-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e9732-126">Request body</span></span>
<span data-ttu-id="e9732-127">В теле запроса добавьте представление объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9732-127">In the request body, supply a JSON representation for the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

<span data-ttu-id="e9732-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="e9732-128">The following table shows the properties that are required when you create the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

|<span data-ttu-id="e9732-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9732-129">Property</span></span>|<span data-ttu-id="e9732-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e9732-130">Type</span></span>|<span data-ttu-id="e9732-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e9732-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9732-132">id</span><span class="sxs-lookup"><span data-stu-id="e9732-132">id</span></span>|<span data-ttu-id="e9732-133">String</span><span class="sxs-lookup"><span data-stu-id="e9732-133">String</span></span>|<span data-ttu-id="e9732-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e9732-134">Key of the entity.</span></span>|
|<span data-ttu-id="e9732-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e9732-135">lastModifiedDateTime</span></span>|<span data-ttu-id="e9732-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9732-136">DateTimeOffset</span></span>|<span data-ttu-id="e9732-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e9732-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="e9732-138">locale</span><span class="sxs-lookup"><span data-stu-id="e9732-138">locale</span></span>|<span data-ttu-id="e9732-139">String</span><span class="sxs-lookup"><span data-stu-id="e9732-139">String</span></span>|<span data-ttu-id="e9732-140">Языковой стандарт, для которого предназначено сообщение.</span><span class="sxs-lookup"><span data-stu-id="e9732-140">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="e9732-141">subject</span><span class="sxs-lookup"><span data-stu-id="e9732-141">subject</span></span>|<span data-ttu-id="e9732-142">String</span><span class="sxs-lookup"><span data-stu-id="e9732-142">String</span></span>|<span data-ttu-id="e9732-143">Тема шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="e9732-143">The Message Template Subject.</span></span>|
|<span data-ttu-id="e9732-144">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="e9732-144">messageTemplate</span></span>|<span data-ttu-id="e9732-145">String</span><span class="sxs-lookup"><span data-stu-id="e9732-145">String</span></span>|<span data-ttu-id="e9732-146">Содержимое шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="e9732-146">The Message Template content.</span></span>|
|<span data-ttu-id="e9732-147">isDefault</span><span class="sxs-lookup"><span data-stu-id="e9732-147">isDefault</span></span>|<span data-ttu-id="e9732-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9732-148">Boolean</span></span>|<span data-ttu-id="e9732-149">Флаг, указывающий, используется ли этот языковой стандарт в качестве базового языка.</span><span class="sxs-lookup"><span data-stu-id="e9732-149">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="e9732-150">Можно устанавливать только этот флаг.</span><span class="sxs-lookup"><span data-stu-id="e9732-150">This flag can only be set.</span></span> <span data-ttu-id="e9732-151">Чтобы снять его, задайте этому свойству значение true для другого локализованного сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="e9732-151">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="e9732-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9732-152">Response</span></span>
<span data-ttu-id="e9732-153">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e9732-153">If successful, this method returns a `200 OK` response code and an updated [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9732-154">Пример</span><span class="sxs-lookup"><span data-stu-id="e9732-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9732-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9732-155">Request</span></span>
<span data-ttu-id="e9732-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9732-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
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

### <a name="response"></a><span data-ttu-id="e9732-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9732-157">Response</span></span>
<span data-ttu-id="e9732-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e9732-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





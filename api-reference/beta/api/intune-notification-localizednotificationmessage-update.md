---
title: Обновление объекта localizedNotificationMessage
description: Обновление свойств объекта localizedNotificationMessage.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0fdd3066f0f5b9228008143409d63ceeeecf5c21
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727768"
---
# <a name="update-localizednotificationmessage"></a><span data-ttu-id="47b9e-103">Обновление объекта localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="47b9e-103">Update localizedNotificationMessage</span></span>

<span data-ttu-id="47b9e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47b9e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47b9e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47b9e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47b9e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47b9e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47b9e-107">Обновление свойств объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="47b9e-107">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47b9e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="47b9e-108">Prerequisites</span></span>
<span data-ttu-id="47b9e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47b9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47b9e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47b9e-111">Permission type</span></span>|<span data-ttu-id="47b9e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="47b9e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47b9e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47b9e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="47b9e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47b9e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="47b9e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47b9e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47b9e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47b9e-116">Not supported.</span></span>|
|<span data-ttu-id="47b9e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47b9e-117">Application</span></span>|<span data-ttu-id="47b9e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47b9e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47b9e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47b9e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="47b9e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="47b9e-120">Request headers</span></span>
|<span data-ttu-id="47b9e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47b9e-121">Header</span></span>|<span data-ttu-id="47b9e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="47b9e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47b9e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47b9e-123">Authorization</span></span>|<span data-ttu-id="47b9e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47b9e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47b9e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="47b9e-125">Accept</span></span>|<span data-ttu-id="47b9e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="47b9e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47b9e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="47b9e-127">Request body</span></span>
<span data-ttu-id="47b9e-128">В теле запроса добавьте представление объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47b9e-128">In the request body, supply a JSON representation for the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

<span data-ttu-id="47b9e-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="47b9e-129">The following table shows the properties that are required when you create the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

|<span data-ttu-id="47b9e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="47b9e-130">Property</span></span>|<span data-ttu-id="47b9e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="47b9e-131">Type</span></span>|<span data-ttu-id="47b9e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="47b9e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47b9e-133">id</span><span class="sxs-lookup"><span data-stu-id="47b9e-133">id</span></span>|<span data-ttu-id="47b9e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="47b9e-134">String</span></span>|<span data-ttu-id="47b9e-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="47b9e-135">Key of the entity.</span></span>|
|<span data-ttu-id="47b9e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="47b9e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="47b9e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47b9e-137">DateTimeOffset</span></span>|<span data-ttu-id="47b9e-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="47b9e-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="47b9e-139">locale</span><span class="sxs-lookup"><span data-stu-id="47b9e-139">locale</span></span>|<span data-ttu-id="47b9e-140">String</span><span class="sxs-lookup"><span data-stu-id="47b9e-140">String</span></span>|<span data-ttu-id="47b9e-141">Языковой стандарт, для которого предназначено сообщение.</span><span class="sxs-lookup"><span data-stu-id="47b9e-141">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="47b9e-142">subject</span><span class="sxs-lookup"><span data-stu-id="47b9e-142">subject</span></span>|<span data-ttu-id="47b9e-143">String</span><span class="sxs-lookup"><span data-stu-id="47b9e-143">String</span></span>|<span data-ttu-id="47b9e-144">Тема шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="47b9e-144">The Message Template Subject.</span></span>|
|<span data-ttu-id="47b9e-145">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="47b9e-145">messageTemplate</span></span>|<span data-ttu-id="47b9e-146">String</span><span class="sxs-lookup"><span data-stu-id="47b9e-146">String</span></span>|<span data-ttu-id="47b9e-147">Содержимое шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="47b9e-147">The Message Template content.</span></span>|
|<span data-ttu-id="47b9e-148">isDefault</span><span class="sxs-lookup"><span data-stu-id="47b9e-148">isDefault</span></span>|<span data-ttu-id="47b9e-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="47b9e-149">Boolean</span></span>|<span data-ttu-id="47b9e-150">Флаг, указывающий, используется ли этот языковой стандарт в качестве базового языка.</span><span class="sxs-lookup"><span data-stu-id="47b9e-150">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="47b9e-151">Можно устанавливать только этот флаг.</span><span class="sxs-lookup"><span data-stu-id="47b9e-151">This flag can only be set.</span></span> <span data-ttu-id="47b9e-152">Чтобы снять его, задайте этому свойству значение true для другого локализованного сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="47b9e-152">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="47b9e-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="47b9e-153">Response</span></span>
<span data-ttu-id="47b9e-154">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="47b9e-154">If successful, this method returns a `200 OK` response code and an updated [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47b9e-155">Пример</span><span class="sxs-lookup"><span data-stu-id="47b9e-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="47b9e-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="47b9e-156">Request</span></span>
<span data-ttu-id="47b9e-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47b9e-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="47b9e-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="47b9e-158">Response</span></span>
<span data-ttu-id="47b9e-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="47b9e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






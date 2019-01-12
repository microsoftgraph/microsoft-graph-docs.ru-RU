---
title: Обновление объекта localizedNotificationMessage
description: Обновление свойств объекта localizedNotificationMessage.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bb008b710b2b3b7635c2deb871d04a7395395de6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924771"
---
# <a name="update-localizednotificationmessage"></a><span data-ttu-id="10e68-103">Обновление объекта localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="10e68-103">Update localizedNotificationMessage</span></span>

> <span data-ttu-id="10e68-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="10e68-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10e68-105">Обновление свойств объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="10e68-105">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="10e68-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="10e68-106">Prerequisites</span></span>
<span data-ttu-id="10e68-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10e68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10e68-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10e68-109">Permission type</span></span>|<span data-ttu-id="10e68-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="10e68-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10e68-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10e68-111">Delegated (work or school account)</span></span>|<span data-ttu-id="10e68-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10e68-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="10e68-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10e68-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10e68-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10e68-114">Not supported.</span></span>|
|<span data-ttu-id="10e68-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10e68-115">Application</span></span>|<span data-ttu-id="10e68-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10e68-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10e68-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10e68-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="10e68-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10e68-118">Request headers</span></span>
|<span data-ttu-id="10e68-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="10e68-119">Header</span></span>|<span data-ttu-id="10e68-120">Значение</span><span class="sxs-lookup"><span data-stu-id="10e68-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10e68-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="10e68-121">Authorization</span></span>|<span data-ttu-id="10e68-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="10e68-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10e68-123">Accept</span><span class="sxs-lookup"><span data-stu-id="10e68-123">Accept</span></span>|<span data-ttu-id="10e68-124">application/json</span><span class="sxs-lookup"><span data-stu-id="10e68-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10e68-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="10e68-125">Request body</span></span>
<span data-ttu-id="10e68-126">В теле запроса добавьте представление объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10e68-126">In the request body, supply a JSON representation for the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

<span data-ttu-id="10e68-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="10e68-127">The following table shows the properties that are required when you create the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

|<span data-ttu-id="10e68-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="10e68-128">Property</span></span>|<span data-ttu-id="10e68-129">Тип</span><span class="sxs-lookup"><span data-stu-id="10e68-129">Type</span></span>|<span data-ttu-id="10e68-130">Описание</span><span class="sxs-lookup"><span data-stu-id="10e68-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10e68-131">id</span><span class="sxs-lookup"><span data-stu-id="10e68-131">id</span></span>|<span data-ttu-id="10e68-132">String</span><span class="sxs-lookup"><span data-stu-id="10e68-132">String</span></span>|<span data-ttu-id="10e68-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="10e68-133">Key of the entity.</span></span>|
|<span data-ttu-id="10e68-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="10e68-134">lastModifiedDateTime</span></span>|<span data-ttu-id="10e68-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10e68-135">DateTimeOffset</span></span>|<span data-ttu-id="10e68-136">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="10e68-136">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="10e68-137">locale</span><span class="sxs-lookup"><span data-stu-id="10e68-137">locale</span></span>|<span data-ttu-id="10e68-138">String</span><span class="sxs-lookup"><span data-stu-id="10e68-138">String</span></span>|<span data-ttu-id="10e68-139">Языковой стандарт, для которого предназначено сообщение.</span><span class="sxs-lookup"><span data-stu-id="10e68-139">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="10e68-140">subject</span><span class="sxs-lookup"><span data-stu-id="10e68-140">subject</span></span>|<span data-ttu-id="10e68-141">String</span><span class="sxs-lookup"><span data-stu-id="10e68-141">String</span></span>|<span data-ttu-id="10e68-142">Тема шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="10e68-142">The Message Template Subject.</span></span>|
|<span data-ttu-id="10e68-143">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="10e68-143">messageTemplate</span></span>|<span data-ttu-id="10e68-144">String</span><span class="sxs-lookup"><span data-stu-id="10e68-144">String</span></span>|<span data-ttu-id="10e68-145">Содержимое шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="10e68-145">The Message Template content.</span></span>|
|<span data-ttu-id="10e68-146">isDefault</span><span class="sxs-lookup"><span data-stu-id="10e68-146">isDefault</span></span>|<span data-ttu-id="10e68-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="10e68-147">Boolean</span></span>|<span data-ttu-id="10e68-148">Флаг, указывающий, используется ли этот языковой стандарт в качестве базового языка.</span><span class="sxs-lookup"><span data-stu-id="10e68-148">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="10e68-149">Можно устанавливать только этот флаг.</span><span class="sxs-lookup"><span data-stu-id="10e68-149">This flag can only be set.</span></span> <span data-ttu-id="10e68-150">Чтобы снять его, задайте этому свойству значение true для другого локализованного сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="10e68-150">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="10e68-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="10e68-151">Response</span></span>
<span data-ttu-id="10e68-152">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="10e68-152">If successful, this method returns a `200 OK` response code and an updated [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10e68-153">Пример</span><span class="sxs-lookup"><span data-stu-id="10e68-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="10e68-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="10e68-154">Request</span></span>
<span data-ttu-id="10e68-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10e68-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="10e68-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="10e68-156">Response</span></span>
<span data-ttu-id="10e68-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="10e68-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




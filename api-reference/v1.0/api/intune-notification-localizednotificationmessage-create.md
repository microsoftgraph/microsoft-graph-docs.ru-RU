---
title: Создание объекта localizedNotificationMessage
description: Создание объекта localizedNotificationMessage.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f257cbce968a97b692993f51faf6794dd0210ae1
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754897"
---
# <a name="create-localizednotificationmessage"></a><span data-ttu-id="886d1-103">Создание объекта localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="886d1-103">Create localizedNotificationMessage</span></span>

<span data-ttu-id="886d1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="886d1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="886d1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="886d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="886d1-106">Создание объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="886d1-106">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="886d1-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="886d1-107">Prerequisites</span></span>
<span data-ttu-id="886d1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="886d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="886d1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="886d1-110">Permission type</span></span>|<span data-ttu-id="886d1-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="886d1-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="886d1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="886d1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="886d1-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="886d1-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="886d1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="886d1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="886d1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="886d1-115">Not supported.</span></span>|
|<span data-ttu-id="886d1-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="886d1-116">Application</span></span>|<span data-ttu-id="886d1-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="886d1-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="886d1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="886d1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="886d1-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="886d1-119">Request headers</span></span>
|<span data-ttu-id="886d1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="886d1-120">Header</span></span>|<span data-ttu-id="886d1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="886d1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="886d1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="886d1-122">Authorization</span></span>|<span data-ttu-id="886d1-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="886d1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="886d1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="886d1-124">Accept</span></span>|<span data-ttu-id="886d1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="886d1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="886d1-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="886d1-126">Request body</span></span>
<span data-ttu-id="886d1-127">В теле запроса добавьте представление объекта localizedNotificationMessage в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="886d1-127">In the request body, supply a JSON representation for the localizedNotificationMessage object.</span></span>

<span data-ttu-id="886d1-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта localizedNotificationMessage.</span><span class="sxs-lookup"><span data-stu-id="886d1-128">The following table shows the properties that are required when you create the localizedNotificationMessage.</span></span>

|<span data-ttu-id="886d1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="886d1-129">Property</span></span>|<span data-ttu-id="886d1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="886d1-130">Type</span></span>|<span data-ttu-id="886d1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="886d1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="886d1-132">id</span><span class="sxs-lookup"><span data-stu-id="886d1-132">id</span></span>|<span data-ttu-id="886d1-133">String</span><span class="sxs-lookup"><span data-stu-id="886d1-133">String</span></span>|<span data-ttu-id="886d1-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="886d1-134">Key of the entity.</span></span>|
|<span data-ttu-id="886d1-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="886d1-135">lastModifiedDateTime</span></span>|<span data-ttu-id="886d1-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="886d1-136">DateTimeOffset</span></span>|<span data-ttu-id="886d1-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="886d1-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="886d1-138">locale</span><span class="sxs-lookup"><span data-stu-id="886d1-138">locale</span></span>|<span data-ttu-id="886d1-139">String</span><span class="sxs-lookup"><span data-stu-id="886d1-139">String</span></span>|<span data-ttu-id="886d1-140">Языковой стандарт, для которого предназначено сообщение.</span><span class="sxs-lookup"><span data-stu-id="886d1-140">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="886d1-141">subject</span><span class="sxs-lookup"><span data-stu-id="886d1-141">subject</span></span>|<span data-ttu-id="886d1-142">String</span><span class="sxs-lookup"><span data-stu-id="886d1-142">String</span></span>|<span data-ttu-id="886d1-143">Тема шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="886d1-143">The Message Template Subject.</span></span>|
|<span data-ttu-id="886d1-144">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="886d1-144">messageTemplate</span></span>|<span data-ttu-id="886d1-145">String</span><span class="sxs-lookup"><span data-stu-id="886d1-145">String</span></span>|<span data-ttu-id="886d1-146">Содержимое шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="886d1-146">The Message Template content.</span></span>|
|<span data-ttu-id="886d1-147">isDefault</span><span class="sxs-lookup"><span data-stu-id="886d1-147">isDefault</span></span>|<span data-ttu-id="886d1-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="886d1-148">Boolean</span></span>|<span data-ttu-id="886d1-149">Флаг, указывающий, используется ли этот языковой стандарт в качестве базового языка.</span><span class="sxs-lookup"><span data-stu-id="886d1-149">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="886d1-150">Можно устанавливать только этот флаг.</span><span class="sxs-lookup"><span data-stu-id="886d1-150">This flag can only be set.</span></span> <span data-ttu-id="886d1-151">Чтобы снять его, задайте этому свойству значение true для другого локализованного сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="886d1-151">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="886d1-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="886d1-152">Response</span></span>
<span data-ttu-id="886d1-153">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="886d1-153">If successful, this method returns a `201 Created` response code and a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="886d1-154">Пример</span><span class="sxs-lookup"><span data-stu-id="886d1-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="886d1-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="886d1-155">Request</span></span>
<span data-ttu-id="886d1-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="886d1-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
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

### <a name="response"></a><span data-ttu-id="886d1-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="886d1-157">Response</span></span>
<span data-ttu-id="886d1-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="886d1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





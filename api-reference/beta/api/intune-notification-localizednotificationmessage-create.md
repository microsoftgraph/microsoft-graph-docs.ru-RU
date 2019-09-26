---
title: Создание объекта localizedNotificationMessage
description: Создание объекта localizedNotificationMessage.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bfb4cc9a711c98e100cec34e3bb682b8bf5e0849
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37191178"
---
# <a name="create-localizednotificationmessage"></a><span data-ttu-id="c7637-103">Создание объекта localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="c7637-103">Create localizedNotificationMessage</span></span>

> <span data-ttu-id="c7637-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7637-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7637-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7637-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7637-106">Создание объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="c7637-106">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7637-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c7637-107">Prerequisites</span></span>
<span data-ttu-id="c7637-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7637-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7637-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7637-110">Permission type</span></span>|<span data-ttu-id="c7637-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7637-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7637-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7637-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c7637-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7637-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c7637-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7637-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7637-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7637-115">Not supported.</span></span>|
|<span data-ttu-id="c7637-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7637-116">Application</span></span>|<span data-ttu-id="c7637-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7637-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7637-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7637-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="c7637-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7637-119">Request headers</span></span>
|<span data-ttu-id="c7637-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c7637-120">Header</span></span>|<span data-ttu-id="c7637-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c7637-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7637-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7637-122">Authorization</span></span>|<span data-ttu-id="c7637-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7637-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7637-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c7637-124">Accept</span></span>|<span data-ttu-id="c7637-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c7637-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7637-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c7637-126">Request body</span></span>
<span data-ttu-id="c7637-127">В теле запроса добавьте представление объекта localizedNotificationMessage в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7637-127">In the request body, supply a JSON representation for the localizedNotificationMessage object.</span></span>

<span data-ttu-id="c7637-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта localizedNotificationMessage.</span><span class="sxs-lookup"><span data-stu-id="c7637-128">The following table shows the properties that are required when you create the localizedNotificationMessage.</span></span>

|<span data-ttu-id="c7637-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7637-129">Property</span></span>|<span data-ttu-id="c7637-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c7637-130">Type</span></span>|<span data-ttu-id="c7637-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c7637-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7637-132">id</span><span class="sxs-lookup"><span data-stu-id="c7637-132">id</span></span>|<span data-ttu-id="c7637-133">Строка</span><span class="sxs-lookup"><span data-stu-id="c7637-133">String</span></span>|<span data-ttu-id="c7637-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c7637-134">Key of the entity.</span></span>|
|<span data-ttu-id="c7637-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7637-135">lastModifiedDateTime</span></span>|<span data-ttu-id="c7637-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7637-136">DateTimeOffset</span></span>|<span data-ttu-id="c7637-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c7637-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="c7637-138">locale</span><span class="sxs-lookup"><span data-stu-id="c7637-138">locale</span></span>|<span data-ttu-id="c7637-139">String.</span><span class="sxs-lookup"><span data-stu-id="c7637-139">String</span></span>|<span data-ttu-id="c7637-140">Языковой стандарт, для которого предназначено сообщение.</span><span class="sxs-lookup"><span data-stu-id="c7637-140">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="c7637-141">subject</span><span class="sxs-lookup"><span data-stu-id="c7637-141">subject</span></span>|<span data-ttu-id="c7637-142">String</span><span class="sxs-lookup"><span data-stu-id="c7637-142">String</span></span>|<span data-ttu-id="c7637-143">Тема шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="c7637-143">The Message Template Subject.</span></span>|
|<span data-ttu-id="c7637-144">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="c7637-144">messageTemplate</span></span>|<span data-ttu-id="c7637-145">String</span><span class="sxs-lookup"><span data-stu-id="c7637-145">String</span></span>|<span data-ttu-id="c7637-146">Содержимое шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="c7637-146">The Message Template content.</span></span>|
|<span data-ttu-id="c7637-147">isDefault</span><span class="sxs-lookup"><span data-stu-id="c7637-147">isDefault</span></span>|<span data-ttu-id="c7637-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="c7637-148">Boolean</span></span>|<span data-ttu-id="c7637-149">Флаг, указывающий, используется ли этот языковой стандарт в качестве базового языка.</span><span class="sxs-lookup"><span data-stu-id="c7637-149">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="c7637-150">Можно устанавливать только этот флаг.</span><span class="sxs-lookup"><span data-stu-id="c7637-150">This flag can only be set.</span></span> <span data-ttu-id="c7637-151">Чтобы снять его, задайте этому свойству значение true для другого локализованного сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="c7637-151">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="c7637-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7637-152">Response</span></span>
<span data-ttu-id="c7637-153">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c7637-153">If successful, this method returns a `201 Created` response code and a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7637-154">Пример</span><span class="sxs-lookup"><span data-stu-id="c7637-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7637-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7637-155">Request</span></span>
<span data-ttu-id="c7637-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7637-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
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

### <a name="response"></a><span data-ttu-id="c7637-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7637-157">Response</span></span>
<span data-ttu-id="c7637-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c7637-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





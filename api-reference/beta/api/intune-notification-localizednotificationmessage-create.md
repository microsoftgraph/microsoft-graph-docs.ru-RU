---
title: Создание объекта localizedNotificationMessage
description: Создание объекта localizedNotificationMessage.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8b57e1121a678f6513d5bef22f529b37fea9e2b4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462756"
---
# <a name="create-localizednotificationmessage"></a><span data-ttu-id="75a0c-103">Создание объекта localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="75a0c-103">Create localizedNotificationMessage</span></span>

<span data-ttu-id="75a0c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="75a0c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75a0c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75a0c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75a0c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="75a0c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75a0c-107">Создание объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="75a0c-107">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75a0c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="75a0c-108">Prerequisites</span></span>
<span data-ttu-id="75a0c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75a0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75a0c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75a0c-111">Permission type</span></span>|<span data-ttu-id="75a0c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="75a0c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75a0c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75a0c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="75a0c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75a0c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="75a0c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75a0c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75a0c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75a0c-116">Not supported.</span></span>|
|<span data-ttu-id="75a0c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75a0c-117">Application</span></span>|<span data-ttu-id="75a0c-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75a0c-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="75a0c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75a0c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="75a0c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="75a0c-120">Request headers</span></span>
|<span data-ttu-id="75a0c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="75a0c-121">Header</span></span>|<span data-ttu-id="75a0c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="75a0c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75a0c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="75a0c-123">Authorization</span></span>|<span data-ttu-id="75a0c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75a0c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75a0c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="75a0c-125">Accept</span></span>|<span data-ttu-id="75a0c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="75a0c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75a0c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75a0c-127">Request body</span></span>
<span data-ttu-id="75a0c-128">В теле запроса добавьте представление объекта localizedNotificationMessage в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75a0c-128">In the request body, supply a JSON representation for the localizedNotificationMessage object.</span></span>

<span data-ttu-id="75a0c-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта localizedNotificationMessage.</span><span class="sxs-lookup"><span data-stu-id="75a0c-129">The following table shows the properties that are required when you create the localizedNotificationMessage.</span></span>

|<span data-ttu-id="75a0c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="75a0c-130">Property</span></span>|<span data-ttu-id="75a0c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="75a0c-131">Type</span></span>|<span data-ttu-id="75a0c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="75a0c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75a0c-133">id</span><span class="sxs-lookup"><span data-stu-id="75a0c-133">id</span></span>|<span data-ttu-id="75a0c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="75a0c-134">String</span></span>|<span data-ttu-id="75a0c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="75a0c-135">Key of the entity.</span></span>|
|<span data-ttu-id="75a0c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="75a0c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="75a0c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75a0c-137">DateTimeOffset</span></span>|<span data-ttu-id="75a0c-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="75a0c-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="75a0c-139">locale</span><span class="sxs-lookup"><span data-stu-id="75a0c-139">locale</span></span>|<span data-ttu-id="75a0c-140">String</span><span class="sxs-lookup"><span data-stu-id="75a0c-140">String</span></span>|<span data-ttu-id="75a0c-141">Языковой стандарт, для которого предназначено сообщение.</span><span class="sxs-lookup"><span data-stu-id="75a0c-141">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="75a0c-142">subject</span><span class="sxs-lookup"><span data-stu-id="75a0c-142">subject</span></span>|<span data-ttu-id="75a0c-143">String</span><span class="sxs-lookup"><span data-stu-id="75a0c-143">String</span></span>|<span data-ttu-id="75a0c-144">Тема шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="75a0c-144">The Message Template Subject.</span></span>|
|<span data-ttu-id="75a0c-145">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="75a0c-145">messageTemplate</span></span>|<span data-ttu-id="75a0c-146">String</span><span class="sxs-lookup"><span data-stu-id="75a0c-146">String</span></span>|<span data-ttu-id="75a0c-147">Содержимое шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="75a0c-147">The Message Template content.</span></span>|
|<span data-ttu-id="75a0c-148">isDefault</span><span class="sxs-lookup"><span data-stu-id="75a0c-148">isDefault</span></span>|<span data-ttu-id="75a0c-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="75a0c-149">Boolean</span></span>|<span data-ttu-id="75a0c-150">Флаг, указывающий, используется ли этот языковой стандарт в качестве базового языка.</span><span class="sxs-lookup"><span data-stu-id="75a0c-150">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="75a0c-151">Можно устанавливать только этот флаг.</span><span class="sxs-lookup"><span data-stu-id="75a0c-151">This flag can only be set.</span></span> <span data-ttu-id="75a0c-152">Чтобы снять его, задайте этому свойству значение true для другого локализованного сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="75a0c-152">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="75a0c-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="75a0c-153">Response</span></span>
<span data-ttu-id="75a0c-154">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="75a0c-154">If successful, this method returns a `201 Created` response code and a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75a0c-155">Пример</span><span class="sxs-lookup"><span data-stu-id="75a0c-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="75a0c-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="75a0c-156">Request</span></span>
<span data-ttu-id="75a0c-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75a0c-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="75a0c-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="75a0c-158">Response</span></span>
<span data-ttu-id="75a0c-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75a0c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






---
title: Создание объекта localizedNotificationMessage
description: Создание объекта localizedNotificationMessage.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 57fc5d1d914ef117d136df7ea9cb5bf1c8a31284
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404234"
---
# <a name="create-localizednotificationmessage"></a><span data-ttu-id="a9b06-103">Создание объекта localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="a9b06-103">Create localizedNotificationMessage</span></span>

> <span data-ttu-id="a9b06-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a9b06-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a9b06-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9b06-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a9b06-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a9b06-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9b06-107">Создание объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="a9b06-107">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9b06-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a9b06-108">Prerequisites</span></span>
<span data-ttu-id="a9b06-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a9b06-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a9b06-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9b06-111">Permission type</span></span>|<span data-ttu-id="a9b06-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9b06-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9b06-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9b06-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a9b06-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9b06-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a9b06-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9b06-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9b06-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9b06-116">Not supported.</span></span>|
|<span data-ttu-id="a9b06-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9b06-117">Application</span></span>|<span data-ttu-id="a9b06-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9b06-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9b06-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9b06-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="a9b06-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a9b06-120">Request headers</span></span>
|<span data-ttu-id="a9b06-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a9b06-121">Header</span></span>|<span data-ttu-id="a9b06-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a9b06-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9b06-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9b06-123">Authorization</span></span>|<span data-ttu-id="a9b06-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a9b06-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9b06-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a9b06-125">Accept</span></span>|<span data-ttu-id="a9b06-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a9b06-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9b06-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a9b06-127">Request body</span></span>
<span data-ttu-id="a9b06-128">В теле запроса добавьте представление объекта localizedNotificationMessage в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9b06-128">In the request body, supply a JSON representation for the localizedNotificationMessage object.</span></span>

<span data-ttu-id="a9b06-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта localizedNotificationMessage.</span><span class="sxs-lookup"><span data-stu-id="a9b06-129">The following table shows the properties that are required when you create the localizedNotificationMessage.</span></span>

|<span data-ttu-id="a9b06-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9b06-130">Property</span></span>|<span data-ttu-id="a9b06-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a9b06-131">Type</span></span>|<span data-ttu-id="a9b06-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a9b06-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9b06-133">id</span><span class="sxs-lookup"><span data-stu-id="a9b06-133">id</span></span>|<span data-ttu-id="a9b06-134">String</span><span class="sxs-lookup"><span data-stu-id="a9b06-134">String</span></span>|<span data-ttu-id="a9b06-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a9b06-135">Key of the entity.</span></span>|
|<span data-ttu-id="a9b06-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9b06-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a9b06-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9b06-137">DateTimeOffset</span></span>|<span data-ttu-id="a9b06-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a9b06-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="a9b06-139">locale</span><span class="sxs-lookup"><span data-stu-id="a9b06-139">locale</span></span>|<span data-ttu-id="a9b06-140">String</span><span class="sxs-lookup"><span data-stu-id="a9b06-140">String</span></span>|<span data-ttu-id="a9b06-141">Языковой стандарт, для которого предназначено сообщение.</span><span class="sxs-lookup"><span data-stu-id="a9b06-141">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="a9b06-142">subject</span><span class="sxs-lookup"><span data-stu-id="a9b06-142">subject</span></span>|<span data-ttu-id="a9b06-143">String</span><span class="sxs-lookup"><span data-stu-id="a9b06-143">String</span></span>|<span data-ttu-id="a9b06-144">Тема шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="a9b06-144">The Message Template Subject.</span></span>|
|<span data-ttu-id="a9b06-145">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="a9b06-145">messageTemplate</span></span>|<span data-ttu-id="a9b06-146">String</span><span class="sxs-lookup"><span data-stu-id="a9b06-146">String</span></span>|<span data-ttu-id="a9b06-147">Содержимое шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="a9b06-147">The Message Template content.</span></span>|
|<span data-ttu-id="a9b06-148">isDefault</span><span class="sxs-lookup"><span data-stu-id="a9b06-148">isDefault</span></span>|<span data-ttu-id="a9b06-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9b06-149">Boolean</span></span>|<span data-ttu-id="a9b06-150">Флаг, указывающий, используется ли этот языковой стандарт в качестве базового языка.</span><span class="sxs-lookup"><span data-stu-id="a9b06-150">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="a9b06-151">Можно устанавливать только этот флаг.</span><span class="sxs-lookup"><span data-stu-id="a9b06-151">This flag can only be set.</span></span> <span data-ttu-id="a9b06-152">Чтобы снять его, задайте этому свойству значение true для другого локализованного сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="a9b06-152">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="a9b06-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9b06-153">Response</span></span>
<span data-ttu-id="a9b06-154">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a9b06-154">If successful, this method returns a `201 Created` response code and a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9b06-155">Пример</span><span class="sxs-lookup"><span data-stu-id="a9b06-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9b06-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9b06-156">Request</span></span>
<span data-ttu-id="a9b06-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9b06-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a9b06-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9b06-158">Response</span></span>
<span data-ttu-id="a9b06-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a9b06-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





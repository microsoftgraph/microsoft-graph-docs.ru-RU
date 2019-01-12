---
title: Обновление объекта localizedNotificationMessage
description: Обновление свойств объекта localizedNotificationMessage.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f8a9cc43deee5b2604d470e516969aa4c845434c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941159"
---
# <a name="update-localizednotificationmessage"></a><span data-ttu-id="9296b-103">Обновление объекта localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="9296b-103">Update localizedNotificationMessage</span></span>

> <span data-ttu-id="9296b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9296b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9296b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9296b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9296b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9296b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9296b-107">Обновление свойств объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="9296b-107">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9296b-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9296b-108">Prerequisites</span></span>
<span data-ttu-id="9296b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9296b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9296b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9296b-111">Permission type</span></span>|<span data-ttu-id="9296b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9296b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9296b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9296b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9296b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9296b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9296b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9296b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9296b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9296b-116">Not supported.</span></span>|
|<span data-ttu-id="9296b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9296b-117">Application</span></span>|<span data-ttu-id="9296b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9296b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9296b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9296b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="9296b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9296b-120">Request headers</span></span>
|<span data-ttu-id="9296b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9296b-121">Header</span></span>|<span data-ttu-id="9296b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9296b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9296b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9296b-123">Authorization</span></span>|<span data-ttu-id="9296b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9296b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9296b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9296b-125">Accept</span></span>|<span data-ttu-id="9296b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9296b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9296b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9296b-127">Request body</span></span>
<span data-ttu-id="9296b-128">В теле запроса добавьте представление объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9296b-128">In the request body, supply a JSON representation for the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

<span data-ttu-id="9296b-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="9296b-129">The following table shows the properties that are required when you create the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

|<span data-ttu-id="9296b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9296b-130">Property</span></span>|<span data-ttu-id="9296b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9296b-131">Type</span></span>|<span data-ttu-id="9296b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9296b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9296b-133">id</span><span class="sxs-lookup"><span data-stu-id="9296b-133">id</span></span>|<span data-ttu-id="9296b-134">String</span><span class="sxs-lookup"><span data-stu-id="9296b-134">String</span></span>|<span data-ttu-id="9296b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9296b-135">Key of the entity.</span></span>|
|<span data-ttu-id="9296b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9296b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9296b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9296b-137">DateTimeOffset</span></span>|<span data-ttu-id="9296b-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9296b-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="9296b-139">locale</span><span class="sxs-lookup"><span data-stu-id="9296b-139">locale</span></span>|<span data-ttu-id="9296b-140">String</span><span class="sxs-lookup"><span data-stu-id="9296b-140">String</span></span>|<span data-ttu-id="9296b-141">Языковой стандарт, для которого предназначено сообщение.</span><span class="sxs-lookup"><span data-stu-id="9296b-141">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="9296b-142">subject</span><span class="sxs-lookup"><span data-stu-id="9296b-142">subject</span></span>|<span data-ttu-id="9296b-143">String</span><span class="sxs-lookup"><span data-stu-id="9296b-143">String</span></span>|<span data-ttu-id="9296b-144">Тема шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="9296b-144">The Message Template Subject.</span></span>|
|<span data-ttu-id="9296b-145">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="9296b-145">messageTemplate</span></span>|<span data-ttu-id="9296b-146">String</span><span class="sxs-lookup"><span data-stu-id="9296b-146">String</span></span>|<span data-ttu-id="9296b-147">Содержимое шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="9296b-147">The Message Template content.</span></span>|
|<span data-ttu-id="9296b-148">isDefault</span><span class="sxs-lookup"><span data-stu-id="9296b-148">isDefault</span></span>|<span data-ttu-id="9296b-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="9296b-149">Boolean</span></span>|<span data-ttu-id="9296b-150">Флаг, указывающий, используется ли этот языковой стандарт в качестве базового языка.</span><span class="sxs-lookup"><span data-stu-id="9296b-150">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="9296b-151">Можно устанавливать только этот флаг.</span><span class="sxs-lookup"><span data-stu-id="9296b-151">This flag can only be set.</span></span> <span data-ttu-id="9296b-152">Чтобы снять его, задайте этому свойству значение true для другого локализованного сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="9296b-152">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="9296b-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="9296b-153">Response</span></span>
<span data-ttu-id="9296b-154">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9296b-154">If successful, this method returns a `200 OK` response code and an updated [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9296b-155">Пример</span><span class="sxs-lookup"><span data-stu-id="9296b-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="9296b-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="9296b-156">Request</span></span>
<span data-ttu-id="9296b-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9296b-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
Content-type: application/json
Content-length: 197

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```

### <a name="response"></a><span data-ttu-id="9296b-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="9296b-158">Response</span></span>
<span data-ttu-id="9296b-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9296b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






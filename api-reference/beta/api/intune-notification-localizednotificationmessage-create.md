---
title: Создание объекта localizedNotificationMessage
description: Создание объекта localizedNotificationMessage.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 555cfa1c6c34a99bf001b9c3b1f462f1a7d3e41c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853977"
---
# <a name="create-localizednotificationmessage"></a><span data-ttu-id="7f8b2-103">Создание объекта localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="7f8b2-103">Create localizedNotificationMessage</span></span>

> <span data-ttu-id="7f8b2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7f8b2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f8b2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f8b2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7f8b2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7f8b2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f8b2-107">Создание объекта [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="7f8b2-107">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7f8b2-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7f8b2-108">Prerequisites</span></span>
<span data-ttu-id="7f8b2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f8b2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f8b2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f8b2-111">Permission type</span></span>|<span data-ttu-id="7f8b2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f8b2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f8b2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f8b2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7f8b2-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f8b2-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7f8b2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f8b2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f8b2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f8b2-116">Not supported.</span></span>|
|<span data-ttu-id="7f8b2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f8b2-117">Application</span></span>|<span data-ttu-id="7f8b2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f8b2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f8b2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f8b2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="7f8b2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f8b2-120">Request headers</span></span>
|<span data-ttu-id="7f8b2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7f8b2-121">Header</span></span>|<span data-ttu-id="7f8b2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7f8b2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f8b2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f8b2-123">Authorization</span></span>|<span data-ttu-id="7f8b2-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7f8b2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f8b2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7f8b2-125">Accept</span></span>|<span data-ttu-id="7f8b2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7f8b2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f8b2-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7f8b2-127">Request body</span></span>
<span data-ttu-id="7f8b2-128">В теле запроса добавьте представление объекта localizedNotificationMessage в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f8b2-128">In the request body, supply a JSON representation for the localizedNotificationMessage object.</span></span>

<span data-ttu-id="7f8b2-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта localizedNotificationMessage.</span><span class="sxs-lookup"><span data-stu-id="7f8b2-129">The following table shows the properties that are required when you create the localizedNotificationMessage.</span></span>

|<span data-ttu-id="7f8b2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f8b2-130">Property</span></span>|<span data-ttu-id="7f8b2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7f8b2-131">Type</span></span>|<span data-ttu-id="7f8b2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7f8b2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f8b2-133">id</span><span class="sxs-lookup"><span data-stu-id="7f8b2-133">id</span></span>|<span data-ttu-id="7f8b2-134">Строка</span><span class="sxs-lookup"><span data-stu-id="7f8b2-134">String</span></span>|<span data-ttu-id="7f8b2-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7f8b2-135">Key of the entity.</span></span>|
|<span data-ttu-id="7f8b2-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f8b2-136">lastModifiedDateTime</span></span>|<span data-ttu-id="7f8b2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f8b2-137">DateTimeOffset</span></span>|<span data-ttu-id="7f8b2-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7f8b2-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="7f8b2-139">locale</span><span class="sxs-lookup"><span data-stu-id="7f8b2-139">locale</span></span>|<span data-ttu-id="7f8b2-140">String</span><span class="sxs-lookup"><span data-stu-id="7f8b2-140">String</span></span>|<span data-ttu-id="7f8b2-141">Языковой стандарт, для которого предназначено сообщение.</span><span class="sxs-lookup"><span data-stu-id="7f8b2-141">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="7f8b2-142">subject</span><span class="sxs-lookup"><span data-stu-id="7f8b2-142">subject</span></span>|<span data-ttu-id="7f8b2-143">String</span><span class="sxs-lookup"><span data-stu-id="7f8b2-143">String</span></span>|<span data-ttu-id="7f8b2-144">Тема шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="7f8b2-144">The Message Template Subject.</span></span>|
|<span data-ttu-id="7f8b2-145">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="7f8b2-145">messageTemplate</span></span>|<span data-ttu-id="7f8b2-146">String</span><span class="sxs-lookup"><span data-stu-id="7f8b2-146">String</span></span>|<span data-ttu-id="7f8b2-147">Содержимое шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="7f8b2-147">The Message Template content.</span></span>|
|<span data-ttu-id="7f8b2-148">isDefault</span><span class="sxs-lookup"><span data-stu-id="7f8b2-148">isDefault</span></span>|<span data-ttu-id="7f8b2-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f8b2-149">Boolean</span></span>|<span data-ttu-id="7f8b2-150">Флаг, указывающий, используется ли этот языковой стандарт в качестве базового языка.</span><span class="sxs-lookup"><span data-stu-id="7f8b2-150">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="7f8b2-151">Можно устанавливать только этот флаг.</span><span class="sxs-lookup"><span data-stu-id="7f8b2-151">This flag can only be set.</span></span> <span data-ttu-id="7f8b2-152">Чтобы снять его, задайте этому свойству значение true для другого локализованного сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="7f8b2-152">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="7f8b2-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f8b2-153">Response</span></span>
<span data-ttu-id="7f8b2-154">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7f8b2-154">If successful, this method returns a `201 Created` response code and a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f8b2-155">Пример</span><span class="sxs-lookup"><span data-stu-id="7f8b2-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="7f8b2-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f8b2-156">Request</span></span>
<span data-ttu-id="7f8b2-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f8b2-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
Content-type: application/json
Content-length: 264

{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```

### <a name="response"></a><span data-ttu-id="7f8b2-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f8b2-158">Response</span></span>
<span data-ttu-id="7f8b2-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7f8b2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






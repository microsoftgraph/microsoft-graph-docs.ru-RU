---
title: Обновление объекта remoteAssistancePartner
description: Обновление свойств объекта remoteAssistancePartner.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ca479230d24e58133865e9ff718a867cb7b969fa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853461"
---
# <a name="update-remoteassistancepartner"></a><span data-ttu-id="0ebb5-103">Обновление объекта remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="0ebb5-103">Update remoteAssistancePartner</span></span>

> <span data-ttu-id="0ebb5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0ebb5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ebb5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ebb5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0ebb5-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0ebb5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ebb5-107">Обновление свойств объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="0ebb5-107">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0ebb5-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0ebb5-108">Prerequisites</span></span>
<span data-ttu-id="0ebb5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ebb5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ebb5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ebb5-111">Permission type</span></span>|<span data-ttu-id="0ebb5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ebb5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ebb5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ebb5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0ebb5-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ebb5-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0ebb5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ebb5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ebb5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ebb5-116">Not supported.</span></span>|
|<span data-ttu-id="0ebb5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ebb5-117">Application</span></span>|<span data-ttu-id="0ebb5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ebb5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ebb5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ebb5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="0ebb5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ebb5-120">Request headers</span></span>
|<span data-ttu-id="0ebb5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0ebb5-121">Header</span></span>|<span data-ttu-id="0ebb5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0ebb5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ebb5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ebb5-123">Authorization</span></span>|<span data-ttu-id="0ebb5-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0ebb5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ebb5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0ebb5-125">Accept</span></span>|<span data-ttu-id="0ebb5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ebb5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ebb5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0ebb5-127">Request body</span></span>
<span data-ttu-id="0ebb5-128">В теле запроса добавьте представление объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ebb5-128">In the request body, supply a JSON representation for the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

<span data-ttu-id="0ebb5-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="0ebb5-129">The following table shows the properties that are required when you create the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>

|<span data-ttu-id="0ebb5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ebb5-130">Property</span></span>|<span data-ttu-id="0ebb5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0ebb5-131">Type</span></span>|<span data-ttu-id="0ebb5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0ebb5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ebb5-133">id</span><span class="sxs-lookup"><span data-stu-id="0ebb5-133">id</span></span>|<span data-ttu-id="0ebb5-134">String</span><span class="sxs-lookup"><span data-stu-id="0ebb5-134">String</span></span>|<span data-ttu-id="0ebb5-135">Уникальный идентификатор партнера.</span><span class="sxs-lookup"><span data-stu-id="0ebb5-135">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="0ebb5-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0ebb5-136">displayName</span></span>|<span data-ttu-id="0ebb5-137">String</span><span class="sxs-lookup"><span data-stu-id="0ebb5-137">String</span></span>|<span data-ttu-id="0ebb5-138">Отображаемое имя партнера.</span><span class="sxs-lookup"><span data-stu-id="0ebb5-138">Display name of the partner.</span></span>|
|<span data-ttu-id="0ebb5-139">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="0ebb5-139">onboardingUrl</span></span>|<span data-ttu-id="0ebb5-140">String</span><span class="sxs-lookup"><span data-stu-id="0ebb5-140">String</span></span>|<span data-ttu-id="0ebb5-141">URL-адрес портала подключения партнера, где администратор может настроить свою службу удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="0ebb5-141">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="0ebb5-142">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="0ebb5-142">onboardingStatus</span></span>|[<span data-ttu-id="0ebb5-143">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="0ebb5-143">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="0ebb5-144">БУДЕТ ОПРЕДЕЛЕНО ПОЗЖЕ.</span><span class="sxs-lookup"><span data-stu-id="0ebb5-144">TBD.</span></span> <span data-ttu-id="0ebb5-145">Возможные значения: `notOnboarded`, `onboarding`, `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="0ebb5-145">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="0ebb5-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="0ebb5-146">lastConnectionDateTime</span></span>|<span data-ttu-id="0ebb5-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ebb5-147">DateTimeOffset</span></span>|<span data-ttu-id="0ebb5-148">Метка времени последнего запроса, отправленного в службу Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="0ebb5-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="0ebb5-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ebb5-149">Response</span></span>
<span data-ttu-id="0ebb5-150">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0ebb5-150">If successful, this method returns a `200 OK` response code and an updated [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ebb5-151">Пример</span><span class="sxs-lookup"><span data-stu-id="0ebb5-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="0ebb5-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ebb5-152">Request</span></span>
<span data-ttu-id="0ebb5-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ebb5-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
Content-type: application/json
Content-length: 204

{
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="0ebb5-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="0ebb5-154">Response</span></span>
<span data-ttu-id="0ebb5-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0ebb5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 315

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "7443c8b9-c8b9-7443-b9c8-4374b9c84374",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```






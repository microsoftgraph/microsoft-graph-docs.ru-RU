---
title: Создание объекта remoteAssistancePartner
description: Создание объекта remoteAssistancePartner.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b1f8306c3ece3b5153a9352c38e41eb89e71d6b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410429"
---
# <a name="create-remoteassistancepartner"></a><span data-ttu-id="f71b6-103">Создание объекта remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="f71b6-103">Create remoteAssistancePartner</span></span>

> <span data-ttu-id="f71b6-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f71b6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f71b6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f71b6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f71b6-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f71b6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f71b6-107">Создание объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="f71b6-107">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f71b6-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f71b6-108">Prerequisites</span></span>
<span data-ttu-id="f71b6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f71b6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f71b6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f71b6-111">Permission type</span></span>|<span data-ttu-id="f71b6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f71b6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f71b6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f71b6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f71b6-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f71b6-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f71b6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f71b6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f71b6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f71b6-116">Not supported.</span></span>|
|<span data-ttu-id="f71b6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f71b6-117">Application</span></span>|<span data-ttu-id="f71b6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f71b6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f71b6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f71b6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="f71b6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f71b6-120">Request headers</span></span>
|<span data-ttu-id="f71b6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f71b6-121">Header</span></span>|<span data-ttu-id="f71b6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f71b6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f71b6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f71b6-123">Authorization</span></span>|<span data-ttu-id="f71b6-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f71b6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f71b6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f71b6-125">Accept</span></span>|<span data-ttu-id="f71b6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f71b6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f71b6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f71b6-127">Request body</span></span>
<span data-ttu-id="f71b6-128">В теле запроса добавьте представление объекта remoteAssistancePartner в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f71b6-128">In the request body, supply a JSON representation for the remoteAssistancePartner object.</span></span>

<span data-ttu-id="f71b6-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта remoteAssistancePartner.</span><span class="sxs-lookup"><span data-stu-id="f71b6-129">The following table shows the properties that are required when you create the remoteAssistancePartner.</span></span>

|<span data-ttu-id="f71b6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f71b6-130">Property</span></span>|<span data-ttu-id="f71b6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f71b6-131">Type</span></span>|<span data-ttu-id="f71b6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f71b6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f71b6-133">id</span><span class="sxs-lookup"><span data-stu-id="f71b6-133">id</span></span>|<span data-ttu-id="f71b6-134">String</span><span class="sxs-lookup"><span data-stu-id="f71b6-134">String</span></span>|<span data-ttu-id="f71b6-135">Уникальный идентификатор партнера.</span><span class="sxs-lookup"><span data-stu-id="f71b6-135">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="f71b6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f71b6-136">displayName</span></span>|<span data-ttu-id="f71b6-137">String</span><span class="sxs-lookup"><span data-stu-id="f71b6-137">String</span></span>|<span data-ttu-id="f71b6-138">Отображаемое имя партнера.</span><span class="sxs-lookup"><span data-stu-id="f71b6-138">Display name of the partner.</span></span>|
|<span data-ttu-id="f71b6-139">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="f71b6-139">onboardingUrl</span></span>|<span data-ttu-id="f71b6-140">String</span><span class="sxs-lookup"><span data-stu-id="f71b6-140">String</span></span>|<span data-ttu-id="f71b6-141">URL-адрес портала подключения партнера, где администратор может настроить свою службу удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="f71b6-141">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="f71b6-142">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="f71b6-142">onboardingStatus</span></span>|[<span data-ttu-id="f71b6-143">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="f71b6-143">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="f71b6-144">БУДЕТ ОПРЕДЕЛЕНО ПОЗЖЕ.</span><span class="sxs-lookup"><span data-stu-id="f71b6-144">TBD.</span></span> <span data-ttu-id="f71b6-145">Возможные значения: `notOnboarded`, `onboarding`, `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="f71b6-145">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="f71b6-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="f71b6-146">lastConnectionDateTime</span></span>|<span data-ttu-id="f71b6-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f71b6-147">DateTimeOffset</span></span>|<span data-ttu-id="f71b6-148">Метка времени последнего запроса, отправленного в службу Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="f71b6-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="f71b6-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="f71b6-149">Response</span></span>
<span data-ttu-id="f71b6-150">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f71b6-150">If successful, this method returns a `201 Created` response code and a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f71b6-151">Пример</span><span class="sxs-lookup"><span data-stu-id="f71b6-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="f71b6-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="f71b6-152">Request</span></span>
<span data-ttu-id="f71b6-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f71b6-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners
Content-type: application/json
Content-length: 266

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="f71b6-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="f71b6-154">Response</span></span>
<span data-ttu-id="f71b6-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f71b6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





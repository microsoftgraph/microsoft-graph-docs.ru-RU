---
title: Создание enrollmentProfile
description: Создание нового объекта enrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bf4133e636cd9eedf7737e2003d1ba733a6e08ec
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934144"
---
# <a name="create-enrollmentprofile"></a><span data-ttu-id="6fae4-103">Создание enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="6fae4-103">Create enrollmentProfile</span></span>

> <span data-ttu-id="6fae4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6fae4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6fae4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fae4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6fae4-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6fae4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6fae4-107">Создание нового объекта [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="6fae4-107">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6fae4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6fae4-108">Prerequisites</span></span>
<span data-ttu-id="6fae4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fae4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fae4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6fae4-111">Permission type</span></span>|<span data-ttu-id="6fae4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6fae4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6fae4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6fae4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6fae4-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fae4-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6fae4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6fae4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fae4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fae4-116">Not supported.</span></span>|
|<span data-ttu-id="6fae4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6fae4-117">Application</span></span>|<span data-ttu-id="6fae4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fae4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6fae4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6fae4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="6fae4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6fae4-120">Request headers</span></span>
|<span data-ttu-id="6fae4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6fae4-121">Header</span></span>|<span data-ttu-id="6fae4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6fae4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6fae4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fae4-123">Authorization</span></span>|<span data-ttu-id="6fae4-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6fae4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6fae4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6fae4-125">Accept</span></span>|<span data-ttu-id="6fae4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6fae4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fae4-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6fae4-127">Request body</span></span>
<span data-ttu-id="6fae4-128">В тексте запроса укажите представление JSON для объекта enrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="6fae4-128">In the request body, supply a JSON representation for the enrollmentProfile object.</span></span>

<span data-ttu-id="6fae4-129">В следующей таблице показаны свойства, которые необходимы для создания enrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="6fae4-129">The following table shows the properties that are required when you create the enrollmentProfile.</span></span>

|<span data-ttu-id="6fae4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6fae4-130">Property</span></span>|<span data-ttu-id="6fae4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6fae4-131">Type</span></span>|<span data-ttu-id="6fae4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6fae4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fae4-133">id</span><span class="sxs-lookup"><span data-stu-id="6fae4-133">id</span></span>|<span data-ttu-id="6fae4-134">Строка</span><span class="sxs-lookup"><span data-stu-id="6fae4-134">String</span></span>|<span data-ttu-id="6fae4-135">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="6fae4-135">The GUID for the object</span></span>|
|<span data-ttu-id="6fae4-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6fae4-136">displayName</span></span>|<span data-ttu-id="6fae4-137">String</span><span class="sxs-lookup"><span data-stu-id="6fae4-137">String</span></span>|<span data-ttu-id="6fae4-138">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="6fae4-138">Name of the profile</span></span>|
|<span data-ttu-id="6fae4-139">описание</span><span class="sxs-lookup"><span data-stu-id="6fae4-139">description</span></span>|<span data-ttu-id="6fae4-140">String</span><span class="sxs-lookup"><span data-stu-id="6fae4-140">String</span></span>|<span data-ttu-id="6fae4-141">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="6fae4-141">Description of the profile</span></span>|
|<span data-ttu-id="6fae4-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="6fae4-142">requiresUserAuthentication</span></span>|<span data-ttu-id="6fae4-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fae4-143">Boolean</span></span>|<span data-ttu-id="6fae4-144">Указывает необходимость проверки подлинности пользователей в профиле</span><span class="sxs-lookup"><span data-stu-id="6fae4-144">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="6fae4-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="6fae4-145">configurationEndpointUrl</span></span>|<span data-ttu-id="6fae4-146">String</span><span class="sxs-lookup"><span data-stu-id="6fae4-146">String</span></span>|<span data-ttu-id="6fae4-147">URL-адрес конечной точки конфигурации для подачи заявок</span><span class="sxs-lookup"><span data-stu-id="6fae4-147">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="6fae4-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="6fae4-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="6fae4-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fae4-149">Boolean</span></span>|<span data-ttu-id="6fae4-150">Указывает на проверку подлинности с Apple помощник по настройке вместо портала компании.</span><span class="sxs-lookup"><span data-stu-id="6fae4-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="6fae4-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="6fae4-151">Response</span></span>
<span data-ttu-id="6fae4-152">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6fae4-152">If successful, this method returns a `201 Created` response code and a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fae4-153">Пример</span><span class="sxs-lookup"><span data-stu-id="6fae4-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="6fae4-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="6fae4-154">Request</span></span>
<span data-ttu-id="6fae4-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6fae4-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 306

{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true
}
```

### <a name="response"></a><span data-ttu-id="6fae4-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="6fae4-156">Response</span></span>
<span data-ttu-id="6fae4-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6fae4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 355

{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "id": "012d8d5e-8d5e-012d-5e8d-2d015e8d2d01",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true
}
```






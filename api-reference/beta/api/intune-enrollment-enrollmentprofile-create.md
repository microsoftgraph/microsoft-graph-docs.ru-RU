---
title: Создание enrollmentProfile
description: Создание нового объекта enrollmentProfile.
author: tfitzmac
ms.openlocfilehash: becfc040bb7fa500a5378f16f50f6bcb2e4f106d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313652"
---
# <a name="create-enrollmentprofile"></a><span data-ttu-id="e9835-103">Создание enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="e9835-103">Create enrollmentProfile</span></span>

> <span data-ttu-id="e9835-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e9835-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e9835-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9835-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e9835-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e9835-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e9835-107">Создание нового объекта [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e9835-107">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e9835-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e9835-108">Prerequisites</span></span>
<span data-ttu-id="e9835-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9835-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9835-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9835-111">Permission type</span></span>|<span data-ttu-id="e9835-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9835-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9835-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9835-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e9835-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9835-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e9835-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9835-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9835-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9835-116">Not supported.</span></span>|
|<span data-ttu-id="e9835-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9835-117">Application</span></span>|<span data-ttu-id="e9835-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9835-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9835-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9835-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="e9835-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9835-120">Request headers</span></span>
|<span data-ttu-id="e9835-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e9835-121">Header</span></span>|<span data-ttu-id="e9835-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e9835-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9835-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e9835-123">Authorization</span></span>|<span data-ttu-id="e9835-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e9835-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9835-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e9835-125">Accept</span></span>|<span data-ttu-id="e9835-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e9835-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9835-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e9835-127">Request body</span></span>
<span data-ttu-id="e9835-128">В тексте запроса укажите представление JSON для объекта enrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="e9835-128">In the request body, supply a JSON representation for the enrollmentProfile object.</span></span>

<span data-ttu-id="e9835-129">В следующей таблице показаны свойства, которые необходимы для создания enrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="e9835-129">The following table shows the properties that are required when you create the enrollmentProfile.</span></span>

|<span data-ttu-id="e9835-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9835-130">Property</span></span>|<span data-ttu-id="e9835-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e9835-131">Type</span></span>|<span data-ttu-id="e9835-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e9835-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9835-133">id</span><span class="sxs-lookup"><span data-stu-id="e9835-133">id</span></span>|<span data-ttu-id="e9835-134">Строка</span><span class="sxs-lookup"><span data-stu-id="e9835-134">String</span></span>|<span data-ttu-id="e9835-135">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="e9835-135">The GUID for the object</span></span>|
|<span data-ttu-id="e9835-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e9835-136">displayName</span></span>|<span data-ttu-id="e9835-137">Строка</span><span class="sxs-lookup"><span data-stu-id="e9835-137">String</span></span>|<span data-ttu-id="e9835-138">Имя профиля</span><span class="sxs-lookup"><span data-stu-id="e9835-138">Name of the profile</span></span>|
|<span data-ttu-id="e9835-139">описание</span><span class="sxs-lookup"><span data-stu-id="e9835-139">description</span></span>|<span data-ttu-id="e9835-140">Строка</span><span class="sxs-lookup"><span data-stu-id="e9835-140">String</span></span>|<span data-ttu-id="e9835-141">Описание профиля</span><span class="sxs-lookup"><span data-stu-id="e9835-141">Description of the profile</span></span>|
|<span data-ttu-id="e9835-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="e9835-142">requiresUserAuthentication</span></span>|<span data-ttu-id="e9835-143">Boolean.</span><span class="sxs-lookup"><span data-stu-id="e9835-143">Boolean</span></span>|<span data-ttu-id="e9835-144">Указывает необходимость проверки подлинности пользователей в профиле</span><span class="sxs-lookup"><span data-stu-id="e9835-144">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="e9835-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="e9835-145">configurationEndpointUrl</span></span>|<span data-ttu-id="e9835-146">String.</span><span class="sxs-lookup"><span data-stu-id="e9835-146">String</span></span>|<span data-ttu-id="e9835-147">URL-адрес конечной точки конфигурации для подачи заявок</span><span class="sxs-lookup"><span data-stu-id="e9835-147">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="e9835-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="e9835-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="e9835-149">Boolean.</span><span class="sxs-lookup"><span data-stu-id="e9835-149">Boolean</span></span>|<span data-ttu-id="e9835-150">Указывает на проверку подлинности с Apple помощник по настройке вместо портала компании.</span><span class="sxs-lookup"><span data-stu-id="e9835-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="e9835-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="e9835-151">Response</span></span>
<span data-ttu-id="e9835-152">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e9835-152">If successful, this method returns a `201 Created` response code and a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9835-153">Пример</span><span class="sxs-lookup"><span data-stu-id="e9835-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="e9835-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9835-154">Request</span></span>
<span data-ttu-id="e9835-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9835-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e9835-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="e9835-156">Response</span></span>
<span data-ttu-id="e9835-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e9835-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






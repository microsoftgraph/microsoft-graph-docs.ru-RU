---
title: Обновление symantecCodeSigningCertificate
description: Обновление свойства объекта symantecCodeSigningCertificate.
author: tfitzmac
ms.openlocfilehash: fe3580f0160c50c2580580ff3515a7842ccf610d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318062"
---
# <a name="update-symanteccodesigningcertificate"></a><span data-ttu-id="c2d42-103">Обновление symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="c2d42-103">Update symantecCodeSigningCertificate</span></span>

> <span data-ttu-id="c2d42-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c2d42-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2d42-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2d42-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c2d42-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c2d42-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c2d42-107">Обновление свойства объекта [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="c2d42-107">Update the properties of a [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c2d42-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c2d42-108">Prerequisites</span></span>
<span data-ttu-id="c2d42-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2d42-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2d42-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2d42-111">Permission type</span></span>|<span data-ttu-id="c2d42-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2d42-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2d42-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2d42-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c2d42-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2d42-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c2d42-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2d42-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2d42-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2d42-116">Not supported.</span></span>|
|<span data-ttu-id="c2d42-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2d42-117">Application</span></span>|<span data-ttu-id="c2d42-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2d42-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2d42-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2d42-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/symantecCodeSigningCertificate
```

## <a name="request-headers"></a><span data-ttu-id="c2d42-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2d42-120">Request headers</span></span>
|<span data-ttu-id="c2d42-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2d42-121">Header</span></span>|<span data-ttu-id="c2d42-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c2d42-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2d42-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2d42-123">Authorization</span></span>|<span data-ttu-id="c2d42-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c2d42-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2d42-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c2d42-125">Accept</span></span>|<span data-ttu-id="c2d42-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c2d42-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2d42-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2d42-127">Request body</span></span>
<span data-ttu-id="c2d42-128">В тексте запроса укажите представление JSON для объекта [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="c2d42-128">In the request body, supply a JSON representation for the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

<span data-ttu-id="c2d42-129">В следующей таблице показаны свойства, которые необходимы для создания [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="c2d42-129">The following table shows the properties that are required when you create the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md).</span></span>

|<span data-ttu-id="c2d42-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2d42-130">Property</span></span>|<span data-ttu-id="c2d42-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c2d42-131">Type</span></span>|<span data-ttu-id="c2d42-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c2d42-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2d42-133">id</span><span class="sxs-lookup"><span data-stu-id="c2d42-133">id</span></span>|<span data-ttu-id="c2d42-134">String</span><span class="sxs-lookup"><span data-stu-id="c2d42-134">String</span></span>|<span data-ttu-id="c2d42-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c2d42-135">The key of the entity.</span></span>|
|<span data-ttu-id="c2d42-136">content</span><span class="sxs-lookup"><span data-stu-id="c2d42-136">content</span></span>|<span data-ttu-id="c2d42-137">Binary</span><span class="sxs-lookup"><span data-stu-id="c2d42-137">Binary</span></span>|<span data-ttu-id="c2d42-138">Сертификат подписи кода Symantec Windows в формате необработанные данные.</span><span class="sxs-lookup"><span data-stu-id="c2d42-138">The Windows Symantec Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="c2d42-139">status</span><span class="sxs-lookup"><span data-stu-id="c2d42-139">status</span></span>|[<span data-ttu-id="c2d42-140">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="c2d42-140">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="c2d42-141">Состояние Cert подготовить к работе или не подготовлен.</span><span class="sxs-lookup"><span data-stu-id="c2d42-141">The Cert Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="c2d42-142">Возможные значения: `notProvisioned`, `provisioned`.</span><span class="sxs-lookup"><span data-stu-id="c2d42-142">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="c2d42-143">password</span><span class="sxs-lookup"><span data-stu-id="c2d42-143">password</span></span>|<span data-ttu-id="c2d42-144">Строка</span><span class="sxs-lookup"><span data-stu-id="c2d42-144">String</span></span>|<span data-ttu-id="c2d42-145">Пароль, необходимый для PFX-файл.</span><span class="sxs-lookup"><span data-stu-id="c2d42-145">The Password required for .pfx file.</span></span>|
|<span data-ttu-id="c2d42-146">subjectName</span><span class="sxs-lookup"><span data-stu-id="c2d42-146">subjectName</span></span>|<span data-ttu-id="c2d42-147">String</span><span class="sxs-lookup"><span data-stu-id="c2d42-147">String</span></span>|<span data-ttu-id="c2d42-148">Имя субъекта для сертификата.</span><span class="sxs-lookup"><span data-stu-id="c2d42-148">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="c2d42-149">subject</span><span class="sxs-lookup"><span data-stu-id="c2d42-149">subject</span></span>|<span data-ttu-id="c2d42-150">Строка</span><span class="sxs-lookup"><span data-stu-id="c2d42-150">String</span></span>|<span data-ttu-id="c2d42-151">Значения субъектов для сертификата.</span><span class="sxs-lookup"><span data-stu-id="c2d42-151">The Subject value for the cert.</span></span>|
|<span data-ttu-id="c2d42-152">Имя поставщика</span><span class="sxs-lookup"><span data-stu-id="c2d42-152">issuerName</span></span>|<span data-ttu-id="c2d42-153">String.</span><span class="sxs-lookup"><span data-stu-id="c2d42-153">String</span></span>|<span data-ttu-id="c2d42-154">Имя поставщика для сертификата.</span><span class="sxs-lookup"><span data-stu-id="c2d42-154">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="c2d42-155">издателя</span><span class="sxs-lookup"><span data-stu-id="c2d42-155">issuer</span></span>|<span data-ttu-id="c2d42-156">String.</span><span class="sxs-lookup"><span data-stu-id="c2d42-156">String</span></span>|<span data-ttu-id="c2d42-157">Значение издателя сертификата.</span><span class="sxs-lookup"><span data-stu-id="c2d42-157">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="c2d42-158">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c2d42-158">expirationDateTime</span></span>|<span data-ttu-id="c2d42-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2d42-159">DateTimeOffset</span></span>|<span data-ttu-id="c2d42-160">Срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="c2d42-160">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="c2d42-161">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="c2d42-161">uploadDateTime</span></span>|<span data-ttu-id="c2d42-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2d42-162">DateTimeOffset</span></span>|<span data-ttu-id="c2d42-163">Тип сертификата подписывания кода как Symantec Cert.</span><span class="sxs-lookup"><span data-stu-id="c2d42-163">The Type of the CodeSigning Cert as Symantec Cert.</span></span>|



## <a name="response"></a><span data-ttu-id="c2d42-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2d42-164">Response</span></span>
<span data-ttu-id="c2d42-165">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c2d42-165">If successful, this method returns a `200 OK` response code and an updated [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2d42-166">Пример</span><span class="sxs-lookup"><span data-stu-id="c2d42-166">Example</span></span>
### <a name="request"></a><span data-ttu-id="c2d42-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2d42-167">Request</span></span>
<span data-ttu-id="c2d42-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2d42-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/symantecCodeSigningCertificate
Content-type: application/json
Content-length: 352

{
  "content": "Y29udGVudA==",
  "status": "provisioned",
  "password": "Password value",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
}
```

### <a name="response"></a><span data-ttu-id="c2d42-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2d42-169">Response</span></span>
<span data-ttu-id="c2d42-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c2d42-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 470

{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
  "id": "00ffe83e-e83e-00ff-3ee8-ff003ee8ff00",
  "content": "Y29udGVudA==",
  "status": "provisioned",
  "password": "Password value",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
}
```






---
title: Обновление организации
description: Обновление свойств объекта organization.
ms.openlocfilehash: 50167db2c2078421894fa86d7b24c0b93351616c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027553"
---
# <a name="update-organization"></a><span data-ttu-id="f1e51-103">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="f1e51-103">Update organization</span></span>

> <span data-ttu-id="f1e51-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f1e51-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1e51-105">Обновление свойств объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="f1e51-105">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f1e51-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f1e51-106">Prerequisites</span></span>
<span data-ttu-id="f1e51-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1e51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1e51-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1e51-109">Permission type</span></span>|<span data-ttu-id="f1e51-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1e51-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1e51-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1e51-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f1e51-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1e51-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f1e51-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1e51-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1e51-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1e51-114">Not supported.</span></span>|
|<span data-ttu-id="f1e51-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1e51-115">Application</span></span>|<span data-ttu-id="f1e51-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1e51-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1e51-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1e51-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="f1e51-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1e51-118">Request headers</span></span>
|<span data-ttu-id="f1e51-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f1e51-119">Header</span></span>|<span data-ttu-id="f1e51-120">Значение</span><span class="sxs-lookup"><span data-stu-id="f1e51-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1e51-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1e51-121">Authorization</span></span>|<span data-ttu-id="f1e51-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f1e51-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1e51-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f1e51-123">Accept</span></span>|<span data-ttu-id="f1e51-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f1e51-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1e51-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f1e51-125">Request body</span></span>
<span data-ttu-id="f1e51-126">В теле запроса добавьте представление объекта [organization](../resources/intune-onboarding-organization.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1e51-126">In the request body, supply a JSON representation for the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

<span data-ttu-id="f1e51-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="f1e51-127">The following table shows the properties that are required when you create the [organization](../resources/intune-onboarding-organization.md).</span></span>

|<span data-ttu-id="f1e51-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1e51-128">Property</span></span>|<span data-ttu-id="f1e51-129">Тип</span><span class="sxs-lookup"><span data-stu-id="f1e51-129">Type</span></span>|<span data-ttu-id="f1e51-130">Описание</span><span class="sxs-lookup"><span data-stu-id="f1e51-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1e51-131">id</span><span class="sxs-lookup"><span data-stu-id="f1e51-131">id</span></span>|<span data-ttu-id="f1e51-132">String</span><span class="sxs-lookup"><span data-stu-id="f1e51-132">String</span></span>|<span data-ttu-id="f1e51-133">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="f1e51-133">The GUID for the object.</span></span>|
|<span data-ttu-id="f1e51-134">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="f1e51-134">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="f1e51-135">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="f1e51-135">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="f1e51-136">Центр управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="f1e51-136">Mobile device management authority.</span></span> <span data-ttu-id="f1e51-137">Возможные значения: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="f1e51-137">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|



## <a name="response"></a><span data-ttu-id="f1e51-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1e51-138">Response</span></span>
<span data-ttu-id="f1e51-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [organization](../resources/intune-onboarding-organization.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f1e51-139">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1e51-140">Пример</span><span class="sxs-lookup"><span data-stu-id="f1e51-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="f1e51-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1e51-141">Request</span></span>
<span data-ttu-id="f1e51-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1e51-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/organization/{organizationId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.organization",
  "mobileDeviceManagementAuthority": "intune"
}
```

### <a name="response"></a><span data-ttu-id="f1e51-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="f1e51-143">Response</span></span>
<span data-ttu-id="f1e51-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="f1e51-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 151

{
  "@odata.type": "#microsoft.graph.organization",
  "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
  "mobileDeviceManagementAuthority": "intune"
}
```




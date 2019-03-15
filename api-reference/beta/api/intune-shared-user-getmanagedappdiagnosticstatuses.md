---
title: Функция getManagedAppDiagnosticStatuses
description: Получает состояние диагностической проверки для определенного пользователя.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9fd3ab289e02c96f112a4abe6b698e8dd6134a2a
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571174"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="40417-103">Функция getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="40417-103">getManagedAppDiagnosticStatuses function</span></span>

> <span data-ttu-id="40417-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="40417-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="40417-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40417-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="40417-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="40417-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40417-107">Получает состояние диагностической проверки для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="40417-107">Gets diagnostics validation status for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="40417-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="40417-108">Prerequisites</span></span>
<span data-ttu-id="40417-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="40417-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="40417-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40417-111">Permission type</span></span>|<span data-ttu-id="40417-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="40417-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40417-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40417-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="40417-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="40417-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="40417-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="40417-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="40417-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40417-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40417-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40417-117">Not supported.</span></span>|
|<span data-ttu-id="40417-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40417-118">Application</span></span>|<span data-ttu-id="40417-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40417-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40417-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40417-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="40417-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40417-121">Request headers</span></span>
|<span data-ttu-id="40417-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="40417-122">Header</span></span>|<span data-ttu-id="40417-123">Значение</span><span class="sxs-lookup"><span data-stu-id="40417-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40417-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40417-124">Authorization</span></span>|<span data-ttu-id="40417-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40417-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40417-126">Accept</span><span class="sxs-lookup"><span data-stu-id="40417-126">Accept</span></span>|<span data-ttu-id="40417-127">application/json</span><span class="sxs-lookup"><span data-stu-id="40417-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40417-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="40417-128">Request body</span></span>
<span data-ttu-id="40417-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="40417-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40417-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="40417-130">Response</span></span>
<span data-ttu-id="40417-131">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="40417-131">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40417-132">Пример</span><span class="sxs-lookup"><span data-stu-id="40417-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="40417-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="40417-133">Request</span></span>
<span data-ttu-id="40417-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40417-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="40417-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="40417-135">Response</span></span>
<span data-ttu-id="40417-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="40417-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "value": [
    {
      "@odata.type": "microsoft.graph.managedAppDiagnosticStatus",
      "validationName": "Validation Name value",
      "state": "State value",
      "mitigationInstruction": "Mitigation Instruction value"
    }
  ]
}
```







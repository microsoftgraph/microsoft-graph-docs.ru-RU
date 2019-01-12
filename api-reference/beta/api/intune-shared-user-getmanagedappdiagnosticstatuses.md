---
title: Функция getManagedAppDiagnosticStatuses
description: Получает состояние диагностической проверки для определенного пользователя.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cb8beac36b1f0892164fad41de4bdc11aee00094
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939891"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="9dfa5-103">Функция getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="9dfa5-103">getManagedAppDiagnosticStatuses function</span></span>

> <span data-ttu-id="9dfa5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9dfa5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9dfa5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dfa5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9dfa5-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9dfa5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9dfa5-107">Получает состояние диагностической проверки для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="9dfa5-107">Gets diagnostics validation status for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9dfa5-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9dfa5-108">Prerequisites</span></span>
<span data-ttu-id="9dfa5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9dfa5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9dfa5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9dfa5-111">Permission type</span></span>|<span data-ttu-id="9dfa5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9dfa5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9dfa5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9dfa5-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9dfa5-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="9dfa5-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="9dfa5-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9dfa5-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9dfa5-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9dfa5-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9dfa5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dfa5-117">Not supported.</span></span>|
|<span data-ttu-id="9dfa5-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9dfa5-118">Application</span></span>|<span data-ttu-id="9dfa5-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dfa5-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9dfa5-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9dfa5-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="9dfa5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9dfa5-121">Request headers</span></span>
|<span data-ttu-id="9dfa5-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9dfa5-122">Header</span></span>|<span data-ttu-id="9dfa5-123">Значение</span><span class="sxs-lookup"><span data-stu-id="9dfa5-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9dfa5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9dfa5-124">Authorization</span></span>|<span data-ttu-id="9dfa5-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9dfa5-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9dfa5-126">Accept</span><span class="sxs-lookup"><span data-stu-id="9dfa5-126">Accept</span></span>|<span data-ttu-id="9dfa5-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9dfa5-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9dfa5-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9dfa5-128">Request body</span></span>
<span data-ttu-id="9dfa5-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9dfa5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9dfa5-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="9dfa5-130">Response</span></span>
<span data-ttu-id="9dfa5-131">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9dfa5-131">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9dfa5-132">Пример</span><span class="sxs-lookup"><span data-stu-id="9dfa5-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="9dfa5-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9dfa5-133">Request</span></span>
<span data-ttu-id="9dfa5-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9dfa5-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="9dfa5-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="9dfa5-135">Response</span></span>
<span data-ttu-id="9dfa5-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9dfa5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







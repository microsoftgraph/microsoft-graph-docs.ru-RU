---
title: Действие uploadDepToken
description: Загружает новый маркер программы регистрации устройства
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 98c663b80ecfbc2fb1641b8db8bb48af9215c885
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417051"
---
# <a name="uploaddeptoken-action"></a><span data-ttu-id="a5cb7-103">Действие uploadDepToken</span><span class="sxs-lookup"><span data-stu-id="a5cb7-103">uploadDepToken action</span></span>

> <span data-ttu-id="a5cb7-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a5cb7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a5cb7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5cb7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a5cb7-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a5cb7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5cb7-107">Загружает новый маркер программы регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="a5cb7-107">Uploads a new Device Enrollment Program token</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5cb7-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="a5cb7-108">Prerequisites</span></span>
<span data-ttu-id="a5cb7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a5cb7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a5cb7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5cb7-111">Permission type</span></span>|<span data-ttu-id="a5cb7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5cb7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5cb7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5cb7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a5cb7-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5cb7-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a5cb7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5cb7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5cb7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5cb7-116">Not supported.</span></span>|
|<span data-ttu-id="a5cb7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5cb7-117">Application</span></span>|<span data-ttu-id="a5cb7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5cb7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5cb7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5cb7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken
```

## <a name="request-headers"></a><span data-ttu-id="a5cb7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5cb7-120">Request headers</span></span>
|<span data-ttu-id="a5cb7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a5cb7-121">Header</span></span>|<span data-ttu-id="a5cb7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a5cb7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5cb7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5cb7-123">Authorization</span></span>|<span data-ttu-id="a5cb7-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a5cb7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5cb7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a5cb7-125">Accept</span></span>|<span data-ttu-id="a5cb7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a5cb7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5cb7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5cb7-127">Request body</span></span>
<span data-ttu-id="a5cb7-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5cb7-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a5cb7-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="a5cb7-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a5cb7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5cb7-130">Property</span></span>|<span data-ttu-id="a5cb7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a5cb7-131">Type</span></span>|<span data-ttu-id="a5cb7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a5cb7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5cb7-133">appleId</span><span class="sxs-lookup"><span data-stu-id="a5cb7-133">appleId</span></span>|<span data-ttu-id="a5cb7-134">String</span><span class="sxs-lookup"><span data-stu-id="a5cb7-134">String</span></span>|<span data-ttu-id="a5cb7-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a5cb7-135">Not yet documented</span></span>|
|<span data-ttu-id="a5cb7-136">depToken</span><span class="sxs-lookup"><span data-stu-id="a5cb7-136">depToken</span></span>|<span data-ttu-id="a5cb7-137">String</span><span class="sxs-lookup"><span data-stu-id="a5cb7-137">String</span></span>|<span data-ttu-id="a5cb7-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a5cb7-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a5cb7-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5cb7-139">Response</span></span>
<span data-ttu-id="a5cb7-140">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a5cb7-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a5cb7-141">Пример</span><span class="sxs-lookup"><span data-stu-id="a5cb7-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5cb7-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5cb7-142">Request</span></span>
<span data-ttu-id="a5cb7-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5cb7-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken

Content-type: application/json
Content-length: 69

{
  "appleId": "Apple Id value",
  "depToken": "Dep Token value"
}
```

### <a name="response"></a><span data-ttu-id="a5cb7-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5cb7-144">Response</span></span>
<span data-ttu-id="a5cb7-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a5cb7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





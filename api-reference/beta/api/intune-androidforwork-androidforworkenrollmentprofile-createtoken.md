---
title: Действие createToken
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6fb2ce0df64ddb94e2488026985f32e7500fb0e5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144228"
---
# <a name="createtoken-action"></a><span data-ttu-id="06deb-103">Действие createToken</span><span class="sxs-lookup"><span data-stu-id="06deb-103">createToken action</span></span>

> <span data-ttu-id="06deb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06deb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06deb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="06deb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06deb-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="06deb-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06deb-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="06deb-107">Prerequisites</span></span>
<span data-ttu-id="06deb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="06deb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="06deb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06deb-110">Permission type</span></span>|<span data-ttu-id="06deb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="06deb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06deb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06deb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="06deb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06deb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="06deb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06deb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06deb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06deb-115">Not supported.</span></span>|
|<span data-ttu-id="06deb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06deb-116">Application</span></span>|<span data-ttu-id="06deb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06deb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06deb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06deb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}/createToken
```

## <a name="request-headers"></a><span data-ttu-id="06deb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06deb-119">Request headers</span></span>
|<span data-ttu-id="06deb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="06deb-120">Header</span></span>|<span data-ttu-id="06deb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="06deb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06deb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="06deb-122">Authorization</span></span>|<span data-ttu-id="06deb-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="06deb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06deb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="06deb-124">Accept</span></span>|<span data-ttu-id="06deb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="06deb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06deb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="06deb-126">Request body</span></span>
<span data-ttu-id="06deb-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="06deb-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="06deb-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="06deb-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="06deb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="06deb-129">Property</span></span>|<span data-ttu-id="06deb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="06deb-130">Type</span></span>|<span data-ttu-id="06deb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="06deb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06deb-132">tokenValidityInSeconds</span><span class="sxs-lookup"><span data-stu-id="06deb-132">tokenValidityInSeconds</span></span>|<span data-ttu-id="06deb-133">Int32</span><span class="sxs-lookup"><span data-stu-id="06deb-133">Int32</span></span>|<span data-ttu-id="06deb-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="06deb-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="06deb-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="06deb-135">Response</span></span>
<span data-ttu-id="06deb-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="06deb-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="06deb-137">Пример</span><span class="sxs-lookup"><span data-stu-id="06deb-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="06deb-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="06deb-138">Request</span></span>
<span data-ttu-id="06deb-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06deb-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}/createToken

Content-type: application/json
Content-length: 35

{
  "tokenValidityInSeconds": 6
}
```

### <a name="response"></a><span data-ttu-id="06deb-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="06deb-140">Response</span></span>
<span data-ttu-id="06deb-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="06deb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





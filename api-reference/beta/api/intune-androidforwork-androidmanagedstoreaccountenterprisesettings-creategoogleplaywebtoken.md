---
title: Действие createGooglePlayWebToken
description: Создает веб-токен, используемый в встраиваемом компоненте.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 75c705344b1e2d281579a0f70c78a025ee430b65
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43418043"
---
# <a name="creategoogleplaywebtoken-action"></a><span data-ttu-id="f45be-103">Действие createGooglePlayWebToken</span><span class="sxs-lookup"><span data-stu-id="f45be-103">createGooglePlayWebToken action</span></span>

<span data-ttu-id="f45be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f45be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f45be-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f45be-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f45be-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f45be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f45be-107">Создает веб-токен, используемый в встраиваемом компоненте.</span><span class="sxs-lookup"><span data-stu-id="f45be-107">Generates a web token that is used in an embeddable component.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f45be-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f45be-108">Prerequisites</span></span>
<span data-ttu-id="f45be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f45be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f45be-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f45be-111">Permission type</span></span>|<span data-ttu-id="f45be-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f45be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f45be-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f45be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f45be-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f45be-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f45be-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f45be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f45be-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f45be-116">Not supported.</span></span>|
|<span data-ttu-id="f45be-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f45be-117">Application</span></span>|<span data-ttu-id="f45be-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f45be-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f45be-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f45be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken
```

## <a name="request-headers"></a><span data-ttu-id="f45be-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f45be-120">Request headers</span></span>
|<span data-ttu-id="f45be-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f45be-121">Header</span></span>|<span data-ttu-id="f45be-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f45be-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f45be-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f45be-123">Authorization</span></span>|<span data-ttu-id="f45be-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f45be-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f45be-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f45be-125">Accept</span></span>|<span data-ttu-id="f45be-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f45be-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f45be-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f45be-127">Request body</span></span>
<span data-ttu-id="f45be-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f45be-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f45be-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="f45be-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f45be-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f45be-130">Property</span></span>|<span data-ttu-id="f45be-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f45be-131">Type</span></span>|<span data-ttu-id="f45be-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f45be-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f45be-133">парентури</span><span class="sxs-lookup"><span data-stu-id="f45be-133">parentUri</span></span>|<span data-ttu-id="f45be-134">String</span><span class="sxs-lookup"><span data-stu-id="f45be-134">String</span></span>|<span data-ttu-id="f45be-135">HTTPS-путь страницы, на которой размещается компонент.</span><span class="sxs-lookup"><span data-stu-id="f45be-135">The https path of the page hosting the component.</span></span>|



## <a name="response"></a><span data-ttu-id="f45be-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f45be-136">Response</span></span>
<span data-ttu-id="f45be-137">При успешном выполнении это действие возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f45be-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f45be-138">Пример</span><span class="sxs-lookup"><span data-stu-id="f45be-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="f45be-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="f45be-139">Request</span></span>
<span data-ttu-id="f45be-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f45be-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken

Content-type: application/json
Content-length: 39

{
  "parentUri": "Parent Uri value"
}
```

### <a name="response"></a><span data-ttu-id="f45be-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="f45be-141">Response</span></span>
<span data-ttu-id="f45be-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f45be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 53

{
  "value": "Create Google Play Web Token value"
}
```




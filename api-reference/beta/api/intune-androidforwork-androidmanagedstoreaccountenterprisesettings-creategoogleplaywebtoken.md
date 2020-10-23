---
title: Действие createGooglePlayWebToken
description: Создает веб-токен, используемый в встраиваемом компоненте.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a32d943fa35b20fbc98c06099e1acc063b7eb8fb
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48701027"
---
# <a name="creategoogleplaywebtoken-action"></a><span data-ttu-id="f3798-103">Действие createGooglePlayWebToken</span><span class="sxs-lookup"><span data-stu-id="f3798-103">createGooglePlayWebToken action</span></span>

<span data-ttu-id="f3798-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3798-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3798-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3798-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3798-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3798-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3798-107">Создает веб-токен, используемый в встраиваемом компоненте.</span><span class="sxs-lookup"><span data-stu-id="f3798-107">Generates a web token that is used in an embeddable component.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3798-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f3798-108">Prerequisites</span></span>
<span data-ttu-id="f3798-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3798-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3798-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3798-111">Permission type</span></span>|<span data-ttu-id="f3798-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3798-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3798-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3798-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f3798-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3798-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f3798-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3798-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3798-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3798-116">Not supported.</span></span>|
|<span data-ttu-id="f3798-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3798-117">Application</span></span>|<span data-ttu-id="f3798-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3798-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3798-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3798-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken
```

## <a name="request-headers"></a><span data-ttu-id="f3798-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f3798-120">Request headers</span></span>
|<span data-ttu-id="f3798-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3798-121">Header</span></span>|<span data-ttu-id="f3798-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f3798-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3798-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3798-123">Authorization</span></span>|<span data-ttu-id="f3798-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3798-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3798-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f3798-125">Accept</span></span>|<span data-ttu-id="f3798-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f3798-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3798-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f3798-127">Request body</span></span>
<span data-ttu-id="f3798-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3798-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f3798-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="f3798-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f3798-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3798-130">Property</span></span>|<span data-ttu-id="f3798-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f3798-131">Type</span></span>|<span data-ttu-id="f3798-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f3798-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3798-133">парентури</span><span class="sxs-lookup"><span data-stu-id="f3798-133">parentUri</span></span>|<span data-ttu-id="f3798-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f3798-134">String</span></span>|<span data-ttu-id="f3798-135">HTTPS-путь страницы, на которой размещается компонент.</span><span class="sxs-lookup"><span data-stu-id="f3798-135">The https path of the page hosting the component.</span></span>|



## <a name="response"></a><span data-ttu-id="f3798-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3798-136">Response</span></span>
<span data-ttu-id="f3798-137">При успешном выполнении это действие возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f3798-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3798-138">Пример</span><span class="sxs-lookup"><span data-stu-id="f3798-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3798-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3798-139">Request</span></span>
<span data-ttu-id="f3798-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3798-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken

Content-type: application/json
Content-length: 39

{
  "parentUri": "Parent Uri value"
}
```

### <a name="response"></a><span data-ttu-id="f3798-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3798-141">Response</span></span>
<span data-ttu-id="f3798-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f3798-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 53

{
  "value": "Create Google Play Web Token value"
}
```






---
title: Действие createGooglePlayWebToken
description: Создает веб-токен, используемый в встраиваемом компоненте.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ef4d99a7a36b7fbe56ca588044ee14534371c7a3
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776838"
---
# <a name="creategoogleplaywebtoken-action"></a><span data-ttu-id="dad4d-103">Действие createGooglePlayWebToken</span><span class="sxs-lookup"><span data-stu-id="dad4d-103">createGooglePlayWebToken action</span></span>

> <span data-ttu-id="dad4d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dad4d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dad4d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dad4d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dad4d-106">Создает веб-токен, используемый в встраиваемом компоненте.</span><span class="sxs-lookup"><span data-stu-id="dad4d-106">Generates a web token that is used in an embeddable component.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dad4d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dad4d-107">Prerequisites</span></span>
<span data-ttu-id="dad4d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dad4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dad4d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dad4d-110">Permission type</span></span>|<span data-ttu-id="dad4d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dad4d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dad4d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dad4d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dad4d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dad4d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dad4d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dad4d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dad4d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dad4d-115">Not supported.</span></span>|
|<span data-ttu-id="dad4d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dad4d-116">Application</span></span>|<span data-ttu-id="dad4d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dad4d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dad4d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dad4d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken
```

## <a name="request-headers"></a><span data-ttu-id="dad4d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dad4d-119">Request headers</span></span>
|<span data-ttu-id="dad4d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dad4d-120">Header</span></span>|<span data-ttu-id="dad4d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="dad4d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dad4d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dad4d-122">Authorization</span></span>|<span data-ttu-id="dad4d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dad4d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dad4d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="dad4d-124">Accept</span></span>|<span data-ttu-id="dad4d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dad4d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dad4d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dad4d-126">Request body</span></span>
<span data-ttu-id="dad4d-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dad4d-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="dad4d-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="dad4d-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="dad4d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="dad4d-129">Property</span></span>|<span data-ttu-id="dad4d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="dad4d-130">Type</span></span>|<span data-ttu-id="dad4d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="dad4d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dad4d-132">Парентури</span><span class="sxs-lookup"><span data-stu-id="dad4d-132">parentUri</span></span>|<span data-ttu-id="dad4d-133">String</span><span class="sxs-lookup"><span data-stu-id="dad4d-133">String</span></span>|<span data-ttu-id="dad4d-134">HTTPS-путь страницы, на которой размещается компонент.</span><span class="sxs-lookup"><span data-stu-id="dad4d-134">The https path of the page hosting the component.</span></span>|



## <a name="response"></a><span data-ttu-id="dad4d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="dad4d-135">Response</span></span>
<span data-ttu-id="dad4d-136">При успешном выполнении это действие возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dad4d-136">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dad4d-137">Пример</span><span class="sxs-lookup"><span data-stu-id="dad4d-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="dad4d-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="dad4d-138">Request</span></span>
<span data-ttu-id="dad4d-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dad4d-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken

Content-type: application/json
Content-length: 39

{
  "parentUri": "Parent Uri value"
}
```

### <a name="response"></a><span data-ttu-id="dad4d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="dad4d-140">Response</span></span>
<span data-ttu-id="dad4d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dad4d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 53

{
  "value": "Create Google Play Web Token value"
}
```






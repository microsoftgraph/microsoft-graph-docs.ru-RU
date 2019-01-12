---
title: Действие createGooglePlayWebToken
description: Создает веб-маркера, который используется в встраиваемые компонента.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 415ac7283f00c0ac79ba0cf480b5a4d24219d84a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956439"
---
# <a name="creategoogleplaywebtoken-action"></a><span data-ttu-id="cc90f-103">Действие createGooglePlayWebToken</span><span class="sxs-lookup"><span data-stu-id="cc90f-103">createGooglePlayWebToken action</span></span>

> <span data-ttu-id="cc90f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cc90f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc90f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc90f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cc90f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cc90f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cc90f-107">Создает веб-маркера, который используется в встраиваемые компонента.</span><span class="sxs-lookup"><span data-stu-id="cc90f-107">Generates a web token that is used in an embeddable component.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cc90f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cc90f-108">Prerequisites</span></span>
<span data-ttu-id="cc90f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc90f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc90f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc90f-111">Permission type</span></span>|<span data-ttu-id="cc90f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc90f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc90f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc90f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cc90f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc90f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cc90f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc90f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc90f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc90f-116">Not supported.</span></span>|
|<span data-ttu-id="cc90f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cc90f-117">Application</span></span>|<span data-ttu-id="cc90f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc90f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc90f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc90f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken
```

## <a name="request-headers"></a><span data-ttu-id="cc90f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc90f-120">Request headers</span></span>
|<span data-ttu-id="cc90f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cc90f-121">Header</span></span>|<span data-ttu-id="cc90f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cc90f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc90f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc90f-123">Authorization</span></span>|<span data-ttu-id="cc90f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="cc90f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc90f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cc90f-125">Accept</span></span>|<span data-ttu-id="cc90f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cc90f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc90f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cc90f-127">Request body</span></span>
<span data-ttu-id="cc90f-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc90f-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="cc90f-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="cc90f-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="cc90f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc90f-130">Property</span></span>|<span data-ttu-id="cc90f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cc90f-131">Type</span></span>|<span data-ttu-id="cc90f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cc90f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc90f-133">parentUri</span><span class="sxs-lookup"><span data-stu-id="cc90f-133">parentUri</span></span>|<span data-ttu-id="cc90f-134">String</span><span class="sxs-lookup"><span data-stu-id="cc90f-134">String</span></span>|<span data-ttu-id="cc90f-135">Https путь к странице, размещающего компонент.</span><span class="sxs-lookup"><span data-stu-id="cc90f-135">The https path of the page hosting the component.</span></span>|



## <a name="response"></a><span data-ttu-id="cc90f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc90f-136">Response</span></span>
<span data-ttu-id="cc90f-137">При успешном выполнении это действие возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cc90f-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc90f-138">Пример</span><span class="sxs-lookup"><span data-stu-id="cc90f-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="cc90f-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc90f-139">Request</span></span>
<span data-ttu-id="cc90f-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc90f-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken

Content-type: application/json
Content-length: 39

{
  "parentUri": "Parent Uri value"
}
```

### <a name="response"></a><span data-ttu-id="cc90f-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc90f-141">Response</span></span>
<span data-ttu-id="cc90f-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="cc90f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 53

{
  "value": "Create Google Play Web Token value"
}
```






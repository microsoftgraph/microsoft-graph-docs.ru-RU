---
title: Удаление Пфксусерцертификате
description: Удаляет объект Пфксусерцертификате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 25e1405b74188eb4c0948bc154bb7d34daf845b5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741483"
---
# <a name="delete-pfxusercertificate"></a><span data-ttu-id="af873-103">Удаление Пфксусерцертификате</span><span class="sxs-lookup"><span data-stu-id="af873-103">Delete pfxUserCertificate</span></span>

> <span data-ttu-id="af873-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af873-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af873-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="af873-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af873-106">Удаляет объект [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md).</span><span class="sxs-lookup"><span data-stu-id="af873-106">Deletes a [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af873-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="af873-107">Prerequisites</span></span>
<span data-ttu-id="af873-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af873-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af873-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af873-110">Permission type</span></span>|<span data-ttu-id="af873-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="af873-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af873-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af873-112">Delegated (work or school account)</span></span>|<span data-ttu-id="af873-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af873-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="af873-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af873-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af873-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af873-115">Not supported.</span></span>|
|<span data-ttu-id="af873-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af873-116">Application</span></span>|<span data-ttu-id="af873-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af873-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af873-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af873-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /pfxUserCertificates/{pfxUserCertificatesId}
```

## <a name="request-headers"></a><span data-ttu-id="af873-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="af873-119">Request headers</span></span>
|<span data-ttu-id="af873-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="af873-120">Header</span></span>|<span data-ttu-id="af873-121">Значение</span><span class="sxs-lookup"><span data-stu-id="af873-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af873-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="af873-122">Authorization</span></span>|<span data-ttu-id="af873-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af873-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af873-124">Accept</span><span class="sxs-lookup"><span data-stu-id="af873-124">Accept</span></span>|<span data-ttu-id="af873-125">application/json</span><span class="sxs-lookup"><span data-stu-id="af873-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af873-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="af873-126">Request body</span></span>
<span data-ttu-id="af873-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="af873-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af873-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="af873-128">Response</span></span>
<span data-ttu-id="af873-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="af873-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="af873-130">Пример</span><span class="sxs-lookup"><span data-stu-id="af873-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="af873-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="af873-131">Request</span></span>
<span data-ttu-id="af873-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af873-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/pfxUserCertificates/{pfxUserCertificatesId}
```

### <a name="response"></a><span data-ttu-id="af873-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="af873-133">Response</span></span>
<span data-ttu-id="af873-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="af873-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






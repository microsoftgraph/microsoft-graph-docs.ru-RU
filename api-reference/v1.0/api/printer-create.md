---
title: 'принтер: создание'
description: Создайте (зарегистрируйте) принтер с помощью службы универсальной печати.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: bd07e04aa2a4c8b459e90a55d537c683a677d8e9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772046"
---
# <a name="printer-create"></a><span data-ttu-id="a4006-103">принтер: создание</span><span class="sxs-lookup"><span data-stu-id="a4006-103">printer: create</span></span>
<span data-ttu-id="a4006-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4006-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="a4006-105">Создайте (зарегистрируйте) принтер с помощью службы универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="a4006-105">Create (register) a printer with the Universal Print service.</span></span> <span data-ttu-id="a4006-106">Это долгосрочная операция, и в качестве таковой возвращается [принтерCreateOperation,](../resources/printercreateoperation.md) который можно использовать для отслеживания и проверки регистрации принтера.</span><span class="sxs-lookup"><span data-stu-id="a4006-106">This is a long-running operation and as such, it returns a [printerCreateOperation](../resources/printercreateoperation.md) that can be used to track and verify the registration of the printer.</span></span>

<span data-ttu-id="a4006-107">Справки по созданию необходимого запроса на подписание сертификатов (CSR) для создания принтера см. в примере кода поколения [CSR.](/universal-print/hardware/universal-print-oem-certificate-signing-request)</span><span class="sxs-lookup"><span data-stu-id="a4006-107">For help creating the required Certificate Signing Request (CSR) for creating printer, see the [CSR generation code sample](/universal-print/hardware/universal-print-oem-certificate-signing-request).</span></span>

## <a name="permissions"></a><span data-ttu-id="a4006-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a4006-108">Permissions</span></span>
<span data-ttu-id="a4006-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4006-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a4006-111">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="a4006-111">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="a4006-112">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="a4006-112">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="a4006-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4006-113">Permission type</span></span> | <span data-ttu-id="a4006-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4006-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="a4006-115">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4006-115">Delegated (work or school account)</span></span>| <span data-ttu-id="a4006-116">Printer.Create, Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="a4006-116">Printer.Create, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="a4006-117">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4006-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4006-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4006-118">Not Supported.</span></span>|
|<span data-ttu-id="a4006-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a4006-119">Application</span></span>| <span data-ttu-id="a4006-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4006-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4006-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4006-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/create
```

## <a name="request-headers"></a><span data-ttu-id="a4006-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4006-122">Request headers</span></span>
|<span data-ttu-id="a4006-123">Имя</span><span class="sxs-lookup"><span data-stu-id="a4006-123">Name</span></span>|<span data-ttu-id="a4006-124">Описание</span><span class="sxs-lookup"><span data-stu-id="a4006-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a4006-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a4006-125">Authorization</span></span>|<span data-ttu-id="a4006-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4006-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a4006-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a4006-128">Content-Type</span></span>|<span data-ttu-id="a4006-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4006-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4006-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4006-131">Request body</span></span>
<span data-ttu-id="a4006-132">В теле запроса поставляем представление JSON параметров.</span><span class="sxs-lookup"><span data-stu-id="a4006-132">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="a4006-133">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="a4006-133">The following table shows the parameters that can be used with this action.</span></span>

| <span data-ttu-id="a4006-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="a4006-134">Parameter</span></span>      | <span data-ttu-id="a4006-135">Тип</span><span class="sxs-lookup"><span data-stu-id="a4006-135">Type</span></span>    |<span data-ttu-id="a4006-136">Описание</span><span class="sxs-lookup"><span data-stu-id="a4006-136">Description</span></span>| <span data-ttu-id="a4006-137">Обязательный?</span><span class="sxs-lookup"><span data-stu-id="a4006-137">Required?</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="a4006-138">displayName</span><span class="sxs-lookup"><span data-stu-id="a4006-138">displayName</span></span>|<span data-ttu-id="a4006-139">String</span><span class="sxs-lookup"><span data-stu-id="a4006-139">String</span></span>|<span data-ttu-id="a4006-140">Имя отображения, которое необходимо назначить принтеру.</span><span class="sxs-lookup"><span data-stu-id="a4006-140">The display name to assign to the printer.</span></span>|<span data-ttu-id="a4006-141">Да</span><span class="sxs-lookup"><span data-stu-id="a4006-141">Yes</span></span>|
|<span data-ttu-id="a4006-142">manufacturer</span><span class="sxs-lookup"><span data-stu-id="a4006-142">manufacturer</span></span>|<span data-ttu-id="a4006-143">String</span><span class="sxs-lookup"><span data-stu-id="a4006-143">String</span></span>|<span data-ttu-id="a4006-144">Производитель принтера.</span><span class="sxs-lookup"><span data-stu-id="a4006-144">The manufacturer of the printer.</span></span>|<span data-ttu-id="a4006-145">Да</span><span class="sxs-lookup"><span data-stu-id="a4006-145">Yes</span></span>|
|<span data-ttu-id="a4006-146">model</span><span class="sxs-lookup"><span data-stu-id="a4006-146">model</span></span>|<span data-ttu-id="a4006-147">String</span><span class="sxs-lookup"><span data-stu-id="a4006-147">String</span></span>|<span data-ttu-id="a4006-148">Модель принтера.</span><span class="sxs-lookup"><span data-stu-id="a4006-148">The model of the printer.</span></span>|<span data-ttu-id="a4006-149">Да</span><span class="sxs-lookup"><span data-stu-id="a4006-149">Yes</span></span>|
|<span data-ttu-id="a4006-150">physicalDeviceId</span><span class="sxs-lookup"><span data-stu-id="a4006-150">physicalDeviceId</span></span>|<span data-ttu-id="a4006-151">String</span><span class="sxs-lookup"><span data-stu-id="a4006-151">String</span></span>|<span data-ttu-id="a4006-152">UUID физического устройства принтера.</span><span class="sxs-lookup"><span data-stu-id="a4006-152">The physical device UUID of the printer.</span></span> <span data-ttu-id="a4006-153">Обязательно, если `hasPhysicalDevice` свойство является верным.</span><span class="sxs-lookup"><span data-stu-id="a4006-153">Required if the `hasPhysicalDevice` property is true.</span></span>|<span data-ttu-id="a4006-154">Нет</span><span class="sxs-lookup"><span data-stu-id="a4006-154">No</span></span>|
|<span data-ttu-id="a4006-155">hasPhysicalDevice</span><span class="sxs-lookup"><span data-stu-id="a4006-155">hasPhysicalDevice</span></span>|<span data-ttu-id="a4006-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4006-156">Boolean</span></span>|<span data-ttu-id="a4006-157">True, если на принтере есть физическое выходное устройство, ложное в противном случае.</span><span class="sxs-lookup"><span data-stu-id="a4006-157">True if the printer has physical output device, false otherwise.</span></span> <span data-ttu-id="a4006-158">Если значение опущено, значение по умолчанию является верным.</span><span class="sxs-lookup"><span data-stu-id="a4006-158">If omitted, the default value is true.</span></span>|<span data-ttu-id="a4006-159">Нет</span><span class="sxs-lookup"><span data-stu-id="a4006-159">No</span></span>|
|<span data-ttu-id="a4006-160">certificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="a4006-160">certificateSigningRequest</span></span>|[<span data-ttu-id="a4006-161">printCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="a4006-161">printCertificateSigningRequest</span></span>](../resources/printcertificatesigningrequest.md)|<span data-ttu-id="a4006-162">Запрос на подписание сертификата X.509 (CSR) для сертификата, созданного и используемой принтером для идентификации.</span><span class="sxs-lookup"><span data-stu-id="a4006-162">The X.509 Certificate Signing Request (CSR) for the certificate created and used by the printer to identify itself.</span></span>|<span data-ttu-id="a4006-163">Да</span><span class="sxs-lookup"><span data-stu-id="a4006-163">Yes</span></span>|
|<span data-ttu-id="a4006-164">connectorId</span><span class="sxs-lookup"><span data-stu-id="a4006-164">connectorId</span></span>|<span data-ttu-id="a4006-165">String</span><span class="sxs-lookup"><span data-stu-id="a4006-165">String</span></span>|<span data-ttu-id="a4006-166">ID соединителя, действующего в качестве прокси-сервера принтера.</span><span class="sxs-lookup"><span data-stu-id="a4006-166">ID of the connector acting as proxy to the printer.</span></span>|<span data-ttu-id="a4006-167">Нет</span><span class="sxs-lookup"><span data-stu-id="a4006-167">No</span></span>|

## <a name="response"></a><span data-ttu-id="a4006-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4006-168">Response</span></span>
<span data-ttu-id="a4006-169">В случае успешного использования этот метод возвращает код отклика и ссылку на связанный `202 Accepted` [принтерCreateOperation](../resources/printercreateoperation.md) в `Operation-Location` загонке.</span><span class="sxs-lookup"><span data-stu-id="a4006-169">If successful, this method returns a `202 Accepted` response code and a link to the associated [printerCreateOperation](../resources/printercreateoperation.md) in the `Operation-Location` header.</span></span>

<span data-ttu-id="a4006-170">Вы делаете запрос GET на связанный URL-адрес, чтобы получить состояние текущей регистрации принтера.</span><span class="sxs-lookup"><span data-stu-id="a4006-170">You make a GET request to the linked URL to get the status of an ongoing printer registration.</span></span> <span data-ttu-id="a4006-171">После успешного завершения регистрации принтера запрос GET на связанный URL-адрес будет содержать созданный объект принтера и зарегистрированный сертификат.</span><span class="sxs-lookup"><span data-stu-id="a4006-171">After printer registration has completed successfully, a GET request to the linked URL will contain the created printer object and registered certificate.</span></span>

## <a name="examples"></a><span data-ttu-id="a4006-172">Примеры</span><span class="sxs-lookup"><span data-stu-id="a4006-172">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a4006-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4006-173">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a4006-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4006-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printer_create"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/create
Content-Type: application/json
Content-length: 287

{
  "displayName": "Test Printer",
  "manufacturer": "Test Printer Manufacturer",
  "model": "Test Printer Model",
  "physicalDeviceId": null,
  "hasPhysicalDevice": false,
  "certificateSigningRequest": { 
    "content": "{content}",
    "transportKey": "{sampleTransportKey}"
  },
  "connectorId": null
}
```
# <a name="c"></a>[<span data-ttu-id="a4006-175">C#</span><span class="sxs-lookup"><span data-stu-id="a4006-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printer-create-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4006-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4006-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printer-create-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4006-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4006-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printer-create-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a4006-178">Java</span><span class="sxs-lookup"><span data-stu-id="a4006-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printer-create-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="a4006-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4006-179">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
Operation-Location: https://graph.microsoft.com/v1.0/print/operations/f221760a-52e8-4c11-b8c5-5dfaef3a49db
Retry-After: 5
```


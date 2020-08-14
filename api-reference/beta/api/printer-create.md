---
title: 'принтер: Create'
description: Создает (регистрирует) принтер с помощью универсальной службы печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: bf100a99d573c186efa64af1692250534a31c50a
ms.sourcegitcommit: 5c3f4a3e2620d1d9e635e09231bbaa73cb0c3cdd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/14/2020
ms.locfileid: "46674094"
---
# <a name="printer-create"></a><span data-ttu-id="0cb0b-103">принтер: Create</span><span class="sxs-lookup"><span data-stu-id="0cb0b-103">printer: create</span></span>

<span data-ttu-id="0cb0b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cb0b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cb0b-105">Создайте (Зарегистрируйте) принтер с помощью универсальной службы печати.</span><span class="sxs-lookup"><span data-stu-id="0cb0b-105">Create (register) a printer with the Universal Print service.</span></span> <span data-ttu-id="0cb0b-106">Это длительно выполняемая операция, которая возвращает объект [принтеркреатеоператион](../resources/printercreateoperation.md) , который можно использовать для отслеживания и проверки регистрации принтера.</span><span class="sxs-lookup"><span data-stu-id="0cb0b-106">This is a long-running operation and as such, it returns a [printerCreateOperation](../resources/printercreateoperation.md) that can be used to track and verify the registration of the printer.</span></span>

## <a name="permissions"></a><span data-ttu-id="0cb0b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0cb0b-107">Permissions</span></span>
<span data-ttu-id="0cb0b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cb0b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0cb0b-110">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="0cb0b-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="0cb0b-111">Пользователь, вошедшего в систему, должен быть [администратором принтера](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="0cb0b-111">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="0cb0b-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0cb0b-112">Permission type</span></span> | <span data-ttu-id="0cb0b-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0cb0b-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="0cb0b-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0cb0b-114">Delegated (work or school account)</span></span>| <span data-ttu-id="0cb0b-115">Printer. Create, Printer. ReadWrite. ALL, Printer. FullControl. ALL</span><span class="sxs-lookup"><span data-stu-id="0cb0b-115">Printer.Create, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="0cb0b-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0cb0b-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cb0b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cb0b-117">Not Supported.</span></span>|
|<span data-ttu-id="0cb0b-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0cb0b-118">Application</span></span>| <span data-ttu-id="0cb0b-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cb0b-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0cb0b-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0cb0b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/create
```
## <a name="request-headers"></a><span data-ttu-id="0cb0b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0cb0b-121">Request headers</span></span>
| <span data-ttu-id="0cb0b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="0cb0b-122">Name</span></span>       | <span data-ttu-id="0cb0b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="0cb0b-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0cb0b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0cb0b-124">Authorization</span></span> | <span data-ttu-id="0cb0b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0cb0b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0cb0b-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0cb0b-127">Content-type</span></span>  | <span data-ttu-id="0cb0b-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0cb0b-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cb0b-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0cb0b-130">Request body</span></span>
<span data-ttu-id="0cb0b-131">В тексте запроса укажите объект JSON со следующими свойствами.</span><span class="sxs-lookup"><span data-stu-id="0cb0b-131">In the request body, provide a JSON object with the following properties.</span></span>

| <span data-ttu-id="0cb0b-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="0cb0b-132">Parameter</span></span>      | <span data-ttu-id="0cb0b-133">Тип</span><span class="sxs-lookup"><span data-stu-id="0cb0b-133">Type</span></span>    |<span data-ttu-id="0cb0b-134">Описание</span><span class="sxs-lookup"><span data-stu-id="0cb0b-134">Description</span></span>| <span data-ttu-id="0cb0b-135">Обязательный?</span><span class="sxs-lookup"><span data-stu-id="0cb0b-135">Required?</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="0cb0b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0cb0b-136">displayName</span></span>|<span data-ttu-id="0cb0b-137">String</span><span class="sxs-lookup"><span data-stu-id="0cb0b-137">String</span></span>|<span data-ttu-id="0cb0b-138">Отображаемое имя, присваиваемое принтеру.</span><span class="sxs-lookup"><span data-stu-id="0cb0b-138">The display name to assign to the printer.</span></span>|<span data-ttu-id="0cb0b-139">Да</span><span class="sxs-lookup"><span data-stu-id="0cb0b-139">Yes</span></span>|
|<span data-ttu-id="0cb0b-140">manufacturer</span><span class="sxs-lookup"><span data-stu-id="0cb0b-140">manufacturer</span></span>|<span data-ttu-id="0cb0b-141">String</span><span class="sxs-lookup"><span data-stu-id="0cb0b-141">String</span></span>|<span data-ttu-id="0cb0b-142">Производитель принтера.</span><span class="sxs-lookup"><span data-stu-id="0cb0b-142">The manufacturer of the printer.</span></span>|<span data-ttu-id="0cb0b-143">Да</span><span class="sxs-lookup"><span data-stu-id="0cb0b-143">Yes</span></span>|
|<span data-ttu-id="0cb0b-144">model</span><span class="sxs-lookup"><span data-stu-id="0cb0b-144">model</span></span>|<span data-ttu-id="0cb0b-145">String</span><span class="sxs-lookup"><span data-stu-id="0cb0b-145">String</span></span>|<span data-ttu-id="0cb0b-146">Модель принтера.</span><span class="sxs-lookup"><span data-stu-id="0cb0b-146">The model of the printer.</span></span>|<span data-ttu-id="0cb0b-147">Да</span><span class="sxs-lookup"><span data-stu-id="0cb0b-147">Yes</span></span>|
|<span data-ttu-id="0cb0b-148">фисикалдевицеид</span><span class="sxs-lookup"><span data-stu-id="0cb0b-148">physicalDeviceId</span></span>|<span data-ttu-id="0cb0b-149">String</span><span class="sxs-lookup"><span data-stu-id="0cb0b-149">String</span></span>|<span data-ttu-id="0cb0b-150">UUID физического устройства принтера.</span><span class="sxs-lookup"><span data-stu-id="0cb0b-150">The physical device UUID of the printer.</span></span> <span data-ttu-id="0cb0b-151">Является обязательным, если `hasPhysicalDevice` свойство имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="0cb0b-151">Required if the `hasPhysicalDevice` property is true.</span></span>|<span data-ttu-id="0cb0b-152">Нет</span><span class="sxs-lookup"><span data-stu-id="0cb0b-152">No</span></span>|
|<span data-ttu-id="0cb0b-153">хасфисикалдевице</span><span class="sxs-lookup"><span data-stu-id="0cb0b-153">hasPhysicalDevice</span></span>|<span data-ttu-id="0cb0b-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cb0b-154">Boolean</span></span>|<span data-ttu-id="0cb0b-155">True, если принтер имеет физическое устройство вывода, в противном случае — значение false.</span><span class="sxs-lookup"><span data-stu-id="0cb0b-155">True if the printer has physical output device, false otherwise.</span></span> <span data-ttu-id="0cb0b-156">Если этот параметр опущен, значение по умолчанию — true.</span><span class="sxs-lookup"><span data-stu-id="0cb0b-156">If omitted, the default value is true.</span></span>|<span data-ttu-id="0cb0b-157">Нет</span><span class="sxs-lookup"><span data-stu-id="0cb0b-157">No</span></span>|
|<span data-ttu-id="0cb0b-158">цертификатесигнингрекуест</span><span class="sxs-lookup"><span data-stu-id="0cb0b-158">certificateSigningRequest</span></span>|[<span data-ttu-id="0cb0b-159">printCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="0cb0b-159">printCertificateSigningRequest</span></span>](../resources/printcertificatesigningrequest.md)|<span data-ttu-id="0cb0b-160">Запрос подписи сертификата X. 509 (CSR) для сертификата, созданного и используемого принтером для идентификации.</span><span class="sxs-lookup"><span data-stu-id="0cb0b-160">The X.509 Certificate Signing Request (CSR) for the certificate created and used by the printer to identify itself.</span></span>|<span data-ttu-id="0cb0b-161">Да</span><span class="sxs-lookup"><span data-stu-id="0cb0b-161">Yes</span></span>|
|<span data-ttu-id="0cb0b-162">коннекторид</span><span class="sxs-lookup"><span data-stu-id="0cb0b-162">connectorId</span></span>|<span data-ttu-id="0cb0b-163">String</span><span class="sxs-lookup"><span data-stu-id="0cb0b-163">String</span></span>|<span data-ttu-id="0cb0b-164">Идентификатор соединителя, который выступает в качестве прокси-сервера для принтера.</span><span class="sxs-lookup"><span data-stu-id="0cb0b-164">Id of Connector acting as proxy to the printer.</span></span>|<span data-ttu-id="0cb0b-165">Нет</span><span class="sxs-lookup"><span data-stu-id="0cb0b-165">No</span></span>|

## <a name="response"></a><span data-ttu-id="0cb0b-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="0cb0b-166">Response</span></span>
<span data-ttu-id="0cb0b-167">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика и ссылку на связанный [принтеркреатеоператион](../resources/printercreateoperation.md) в `Operation-Location` заголовке.</span><span class="sxs-lookup"><span data-stu-id="0cb0b-167">If successful, this method returns a `202 Accepted` response code and a link to the associated [printerCreateOperation](../resources/printercreateoperation.md) in the `Operation-Location` header.</span></span>

<span data-ttu-id="0cb0b-168">Чтобы получить состояние текущей регистрации принтера, можно использовать запрос GET к связанному URL-адресу.</span><span class="sxs-lookup"><span data-stu-id="0cb0b-168">Making a GET request to the linked URL can be used to get the status of an ongoing printer registration.</span></span> <span data-ttu-id="0cb0b-169">После успешного завершения регистрации принтера запрос GET к связанному URL-адресу будет содержать созданный объект Printer и зарегистрированный сертификат.</span><span class="sxs-lookup"><span data-stu-id="0cb0b-169">Once printer registration has completed successfully, a GET request to the linked URL will contain the created printer object and registered certificate.</span></span>

## <a name="example"></a><span data-ttu-id="0cb0b-170">Пример</span><span class="sxs-lookup"><span data-stu-id="0cb0b-170">Example</span></span>
### <a name="request"></a><span data-ttu-id="0cb0b-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="0cb0b-171">Request</span></span>
<span data-ttu-id="0cb0b-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0cb0b-172">The following is an example of the request.</span></span> <span data-ttu-id="0cb0b-173">Для получения справки по созданию необходимого запроса подписи сертификата (CSR) обратитесь к [образцу кода создания CSR](https://docs.microsoft.com/universal-print/hardware/universal-print-oem-certificate-signing-request).</span><span class="sxs-lookup"><span data-stu-id="0cb0b-173">For help creating the required Certificate Signing Request (CSR), see the [CSR generation code sample](https://docs.microsoft.com/universal-print/hardware/universal-print-oem-certificate-signing-request).</span></span>


# <a name="http"></a>[<span data-ttu-id="0cb0b-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="0cb0b-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printer"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/create
Content-type: application/json
Content-length: 319

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
# <a name="javascript"></a>[<span data-ttu-id="0cb0b-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0cb0b-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="0cb0b-176">C#</span><span class="sxs-lookup"><span data-stu-id="0cb0b-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0cb0b-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0cb0b-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0cb0b-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="0cb0b-178">Response</span></span>
<span data-ttu-id="0cb0b-179">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0cb0b-179">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
Operation-Location: https://graph.microsoft.com/beta/print/operations/f221760a-52e8-4c11-b8c5-5dfaef3a49db
Retry-After: 5
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printers: create",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

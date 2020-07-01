---
title: 'принтер: Create'
description: Создает (регистрирует) принтер с помощью универсальной службы печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 1b36a856a73d78b479270138868285a852d6d187
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007196"
---
# <a name="printer-create"></a><span data-ttu-id="18e2c-103">принтер: Create</span><span class="sxs-lookup"><span data-stu-id="18e2c-103">printer: create</span></span>

<span data-ttu-id="18e2c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18e2c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18e2c-105">Создайте (Зарегистрируйте) принтер с помощью универсальной службы печати.</span><span class="sxs-lookup"><span data-stu-id="18e2c-105">Create (register) a printer with the Universal Print service.</span></span> <span data-ttu-id="18e2c-106">Это длительно выполняемая операция, которая возвращает объект [принтеркреатеоператион](../resources/printercreateoperation.md) , который можно использовать для отслеживания и проверки регистрации принтера.</span><span class="sxs-lookup"><span data-stu-id="18e2c-106">This is a long-running operation and as such, it returns a [printerCreateOperation](../resources/printercreateoperation.md) that can be used to track and verify the registration of the printer.</span></span>

## <a name="permissions"></a><span data-ttu-id="18e2c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="18e2c-107">Permissions</span></span>
<span data-ttu-id="18e2c-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="18e2c-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="18e2c-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18e2c-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="18e2c-110">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="18e2c-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="18e2c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18e2c-111">Permission type</span></span> | <span data-ttu-id="18e2c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="18e2c-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="18e2c-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18e2c-113">Delegated (work or school account)</span></span>| <span data-ttu-id="18e2c-114">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="18e2c-114">User.Read.All</span></span> |
|<span data-ttu-id="18e2c-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18e2c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18e2c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18e2c-116">Not Supported.</span></span>|
|<span data-ttu-id="18e2c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18e2c-117">Application</span></span>|<span data-ttu-id="18e2c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18e2c-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18e2c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18e2c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/create
```
## <a name="request-headers"></a><span data-ttu-id="18e2c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18e2c-120">Request headers</span></span>
| <span data-ttu-id="18e2c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="18e2c-121">Name</span></span>       | <span data-ttu-id="18e2c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="18e2c-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="18e2c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="18e2c-123">Authorization</span></span> | <span data-ttu-id="18e2c-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="18e2c-124">Bearer {token}.</span></span> <span data-ttu-id="18e2c-125">Required.</span><span class="sxs-lookup"><span data-stu-id="18e2c-125">Required.</span></span> |
| <span data-ttu-id="18e2c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18e2c-126">Content-type</span></span>  | <span data-ttu-id="18e2c-127">application/json.</span><span class="sxs-lookup"><span data-stu-id="18e2c-127">application/json.</span></span> <span data-ttu-id="18e2c-128">Required.</span><span class="sxs-lookup"><span data-stu-id="18e2c-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="18e2c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18e2c-129">Request body</span></span>
<span data-ttu-id="18e2c-130">В тексте запроса укажите объект JSON со следующими свойствами.</span><span class="sxs-lookup"><span data-stu-id="18e2c-130">In the request body, provide a JSON object with the following properties.</span></span>

| <span data-ttu-id="18e2c-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="18e2c-131">Parameter</span></span>      | <span data-ttu-id="18e2c-132">Тип</span><span class="sxs-lookup"><span data-stu-id="18e2c-132">Type</span></span>    |<span data-ttu-id="18e2c-133">Описание</span><span class="sxs-lookup"><span data-stu-id="18e2c-133">Description</span></span>| <span data-ttu-id="18e2c-134">Обязательный?</span><span class="sxs-lookup"><span data-stu-id="18e2c-134">Required?</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="18e2c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="18e2c-135">displayName</span></span>|<span data-ttu-id="18e2c-136">String</span><span class="sxs-lookup"><span data-stu-id="18e2c-136">String</span></span>|<span data-ttu-id="18e2c-137">Отображаемое имя, присваиваемое принтеру.</span><span class="sxs-lookup"><span data-stu-id="18e2c-137">The display name to assign to the printer.</span></span>|<span data-ttu-id="18e2c-138">Да</span><span class="sxs-lookup"><span data-stu-id="18e2c-138">Yes</span></span>|
|<span data-ttu-id="18e2c-139">manufacturer</span><span class="sxs-lookup"><span data-stu-id="18e2c-139">manufacturer</span></span>|<span data-ttu-id="18e2c-140">String</span><span class="sxs-lookup"><span data-stu-id="18e2c-140">String</span></span>|<span data-ttu-id="18e2c-141">Производитель принтера.</span><span class="sxs-lookup"><span data-stu-id="18e2c-141">The manufacturer of the printer.</span></span>|<span data-ttu-id="18e2c-142">Да</span><span class="sxs-lookup"><span data-stu-id="18e2c-142">Yes</span></span>|
|<span data-ttu-id="18e2c-143">model</span><span class="sxs-lookup"><span data-stu-id="18e2c-143">model</span></span>|<span data-ttu-id="18e2c-144">String</span><span class="sxs-lookup"><span data-stu-id="18e2c-144">String</span></span>|<span data-ttu-id="18e2c-145">Модель принтера.</span><span class="sxs-lookup"><span data-stu-id="18e2c-145">The model of the printer.</span></span>|<span data-ttu-id="18e2c-146">Да</span><span class="sxs-lookup"><span data-stu-id="18e2c-146">Yes</span></span>|
|<span data-ttu-id="18e2c-147">фисикалдевицеид</span><span class="sxs-lookup"><span data-stu-id="18e2c-147">physicalDeviceId</span></span>|<span data-ttu-id="18e2c-148">String</span><span class="sxs-lookup"><span data-stu-id="18e2c-148">String</span></span>|<span data-ttu-id="18e2c-149">UUID физического устройства принтера.</span><span class="sxs-lookup"><span data-stu-id="18e2c-149">The physical device UUID of the printer.</span></span> <span data-ttu-id="18e2c-150">Является обязательным, если `hasPhysicalDevice` свойство имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="18e2c-150">Required if the `hasPhysicalDevice` property is true.</span></span>|<span data-ttu-id="18e2c-151">Нет</span><span class="sxs-lookup"><span data-stu-id="18e2c-151">No</span></span>|
|<span data-ttu-id="18e2c-152">хасфисикалдевице</span><span class="sxs-lookup"><span data-stu-id="18e2c-152">hasPhysicalDevice</span></span>|<span data-ttu-id="18e2c-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="18e2c-153">Boolean</span></span>|<span data-ttu-id="18e2c-154">True, если принтер имеет физическое устройство вывода, в противном случае — значение false.</span><span class="sxs-lookup"><span data-stu-id="18e2c-154">True if the printer has physical output device, false otherwise.</span></span> <span data-ttu-id="18e2c-155">Если этот параметр опущен, значение по умолчанию — true.</span><span class="sxs-lookup"><span data-stu-id="18e2c-155">If omitted, the default value is true.</span></span>|<span data-ttu-id="18e2c-156">Нет</span><span class="sxs-lookup"><span data-stu-id="18e2c-156">No</span></span>|
|<span data-ttu-id="18e2c-157">цертификатесигнингрекуест</span><span class="sxs-lookup"><span data-stu-id="18e2c-157">certificateSigningRequest</span></span>|[<span data-ttu-id="18e2c-158">принтцертификатесигнингрекуест</span><span class="sxs-lookup"><span data-stu-id="18e2c-158">printCertificateSigningRequest</span></span>](../resources/printcertificatesigningrequest.md)|<span data-ttu-id="18e2c-159">Запрос подписи сертификата X. 509 (CSR) для сертификата, созданного и используемого принтером для идентификации.</span><span class="sxs-lookup"><span data-stu-id="18e2c-159">The X.509 Certificate Signing Request (CSR) for the certificate created and used by the printer to identify itself.</span></span>|<span data-ttu-id="18e2c-160">Да</span><span class="sxs-lookup"><span data-stu-id="18e2c-160">Yes</span></span>|
|<span data-ttu-id="18e2c-161">коннекторид</span><span class="sxs-lookup"><span data-stu-id="18e2c-161">connectorId</span></span>|<span data-ttu-id="18e2c-162">String</span><span class="sxs-lookup"><span data-stu-id="18e2c-162">String</span></span>|<span data-ttu-id="18e2c-163">Идентификатор соединителя, который выступает в качестве прокси-сервера для принтера.</span><span class="sxs-lookup"><span data-stu-id="18e2c-163">Id of Connector acting as proxy to the printer.</span></span>|<span data-ttu-id="18e2c-164">Нет</span><span class="sxs-lookup"><span data-stu-id="18e2c-164">No</span></span>|

## <a name="response"></a><span data-ttu-id="18e2c-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="18e2c-165">Response</span></span>
<span data-ttu-id="18e2c-166">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика и ссылку на связанный [принтеркреатеоператион](../resources/printercreateoperation.md) в `Operation-Location` заголовке.</span><span class="sxs-lookup"><span data-stu-id="18e2c-166">If successful, this method returns a `202 Accepted` response code and a link to the associated [printerCreateOperation](../resources/printercreateoperation.md) in the `Operation-Location` header.</span></span>

<span data-ttu-id="18e2c-167">Чтобы получить состояние текущей регистрации принтера, можно использовать запрос GET к связанному URL-адресу.</span><span class="sxs-lookup"><span data-stu-id="18e2c-167">Making a GET request to the linked URL can be used to get the status of an ongoing printer registration.</span></span> <span data-ttu-id="18e2c-168">После успешного завершения регистрации принтера запрос GET к связанному URL-адресу будет содержать созданный объект Printer и зарегистрированный сертификат.</span><span class="sxs-lookup"><span data-stu-id="18e2c-168">Once printer registration has completed successfully, a GET request to the linked URL will contain the created printer object and registered certificate.</span></span>

## <a name="example"></a><span data-ttu-id="18e2c-169">Пример</span><span class="sxs-lookup"><span data-stu-id="18e2c-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="18e2c-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="18e2c-170">Request</span></span>
<span data-ttu-id="18e2c-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18e2c-171">The following is an example of the request.</span></span> <span data-ttu-id="18e2c-172">Для получения справки по созданию необходимого запроса подписи сертификата (CSR) обратитесь к [образцу кода создания CSR](https://docs.microsoft.com/universal-print/hardware/universal-print-oem-certificate-signing-request).</span><span class="sxs-lookup"><span data-stu-id="18e2c-172">For help creating the required Certificate Signing Request (CSR), see the [CSR generation code sample](https://docs.microsoft.com/universal-print/hardware/universal-print-oem-certificate-signing-request).</span></span>

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

### <a name="response"></a><span data-ttu-id="18e2c-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="18e2c-173">Response</span></span>
<span data-ttu-id="18e2c-174">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="18e2c-174">The following is an example of the response.</span></span>

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

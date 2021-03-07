---
title: 'принтер: создание'
description: Создайте (зарегистрируйте) принтер с помощью службы универсальной печати.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 58285c3c6908812edce8ad80915f44f4df08fcb8
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517475"
---
# <a name="printer-create"></a><span data-ttu-id="f8101-103">принтер: создание</span><span class="sxs-lookup"><span data-stu-id="f8101-103">printer: create</span></span>
<span data-ttu-id="f8101-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8101-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="f8101-105">Создайте (зарегистрируйте) принтер с помощью службы универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="f8101-105">Create (register) a printer with the Universal Print service.</span></span> <span data-ttu-id="f8101-106">Это долгосрочная операция, и в качестве таковой возвращается [принтерCreateOperation,](../resources/printercreateoperation.md) который можно использовать для отслеживания и проверки регистрации принтера.</span><span class="sxs-lookup"><span data-stu-id="f8101-106">This is a long-running operation and as such, it returns a [printerCreateOperation](../resources/printercreateoperation.md) that can be used to track and verify the registration of the printer.</span></span>

<span data-ttu-id="f8101-107">Справки по созданию необходимого запроса на подписание сертификатов (CSR) для создания принтера см. в примере кода поколения [CSR.](/universal-print/hardware/universal-print-oem-certificate-signing-request)</span><span class="sxs-lookup"><span data-stu-id="f8101-107">For help creating the required Certificate Signing Request (CSR) for creating printer, see the [CSR generation code sample](/universal-print/hardware/universal-print-oem-certificate-signing-request).</span></span>

## <a name="permissions"></a><span data-ttu-id="f8101-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f8101-108">Permissions</span></span>
<span data-ttu-id="f8101-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8101-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f8101-111">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="f8101-111">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="f8101-112">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="f8101-112">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="f8101-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8101-113">Permission type</span></span> | <span data-ttu-id="f8101-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8101-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="f8101-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8101-115">Delegated (work or school account)</span></span>| <span data-ttu-id="f8101-116">Printer.Create, Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="f8101-116">Printer.Create, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="f8101-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8101-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8101-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8101-118">Not Supported.</span></span>|
|<span data-ttu-id="f8101-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8101-119">Application</span></span>| <span data-ttu-id="f8101-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8101-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8101-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8101-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/create
```

## <a name="request-headers"></a><span data-ttu-id="f8101-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f8101-122">Request headers</span></span>
|<span data-ttu-id="f8101-123">Имя</span><span class="sxs-lookup"><span data-stu-id="f8101-123">Name</span></span>|<span data-ttu-id="f8101-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f8101-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f8101-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f8101-125">Authorization</span></span>|<span data-ttu-id="f8101-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f8101-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f8101-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f8101-128">Content-Type</span></span>|<span data-ttu-id="f8101-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f8101-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8101-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f8101-131">Request body</span></span>
<span data-ttu-id="f8101-132">В теле запроса поставляем представление JSON параметров.</span><span class="sxs-lookup"><span data-stu-id="f8101-132">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="f8101-133">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="f8101-133">The following table shows the parameters that can be used with this action.</span></span>

| <span data-ttu-id="f8101-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="f8101-134">Parameter</span></span>      | <span data-ttu-id="f8101-135">Тип</span><span class="sxs-lookup"><span data-stu-id="f8101-135">Type</span></span>    |<span data-ttu-id="f8101-136">Описание</span><span class="sxs-lookup"><span data-stu-id="f8101-136">Description</span></span>| <span data-ttu-id="f8101-137">Обязательный?</span><span class="sxs-lookup"><span data-stu-id="f8101-137">Required?</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="f8101-138">displayName</span><span class="sxs-lookup"><span data-stu-id="f8101-138">displayName</span></span>|<span data-ttu-id="f8101-139">Строка</span><span class="sxs-lookup"><span data-stu-id="f8101-139">String</span></span>|<span data-ttu-id="f8101-140">Имя отображения, которое необходимо назначить принтеру.</span><span class="sxs-lookup"><span data-stu-id="f8101-140">The display name to assign to the printer.</span></span>|<span data-ttu-id="f8101-141">Да</span><span class="sxs-lookup"><span data-stu-id="f8101-141">Yes</span></span>|
|<span data-ttu-id="f8101-142">manufacturer</span><span class="sxs-lookup"><span data-stu-id="f8101-142">manufacturer</span></span>|<span data-ttu-id="f8101-143">String</span><span class="sxs-lookup"><span data-stu-id="f8101-143">String</span></span>|<span data-ttu-id="f8101-144">Производитель принтера.</span><span class="sxs-lookup"><span data-stu-id="f8101-144">The manufacturer of the printer.</span></span>|<span data-ttu-id="f8101-145">Да</span><span class="sxs-lookup"><span data-stu-id="f8101-145">Yes</span></span>|
|<span data-ttu-id="f8101-146">model</span><span class="sxs-lookup"><span data-stu-id="f8101-146">model</span></span>|<span data-ttu-id="f8101-147">String</span><span class="sxs-lookup"><span data-stu-id="f8101-147">String</span></span>|<span data-ttu-id="f8101-148">Модель принтера.</span><span class="sxs-lookup"><span data-stu-id="f8101-148">The model of the printer.</span></span>|<span data-ttu-id="f8101-149">Да</span><span class="sxs-lookup"><span data-stu-id="f8101-149">Yes</span></span>|
|<span data-ttu-id="f8101-150">physicalDeviceId</span><span class="sxs-lookup"><span data-stu-id="f8101-150">physicalDeviceId</span></span>|<span data-ttu-id="f8101-151">Строка</span><span class="sxs-lookup"><span data-stu-id="f8101-151">String</span></span>|<span data-ttu-id="f8101-152">UUID физического устройства принтера.</span><span class="sxs-lookup"><span data-stu-id="f8101-152">The physical device UUID of the printer.</span></span> <span data-ttu-id="f8101-153">Обязательно, если `hasPhysicalDevice` свойство является верным.</span><span class="sxs-lookup"><span data-stu-id="f8101-153">Required if the `hasPhysicalDevice` property is true.</span></span>|<span data-ttu-id="f8101-154">Нет</span><span class="sxs-lookup"><span data-stu-id="f8101-154">No</span></span>|
|<span data-ttu-id="f8101-155">hasPhysicalDevice</span><span class="sxs-lookup"><span data-stu-id="f8101-155">hasPhysicalDevice</span></span>|<span data-ttu-id="f8101-156">Логический</span><span class="sxs-lookup"><span data-stu-id="f8101-156">Boolean</span></span>|<span data-ttu-id="f8101-157">True, если на принтере есть физическое выходное устройство, ложное в противном случае.</span><span class="sxs-lookup"><span data-stu-id="f8101-157">True if the printer has physical output device, false otherwise.</span></span> <span data-ttu-id="f8101-158">Если значение опущено, значение по умолчанию является верным.</span><span class="sxs-lookup"><span data-stu-id="f8101-158">If omitted, the default value is true.</span></span>|<span data-ttu-id="f8101-159">Нет</span><span class="sxs-lookup"><span data-stu-id="f8101-159">No</span></span>|
|<span data-ttu-id="f8101-160">certificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="f8101-160">certificateSigningRequest</span></span>|[<span data-ttu-id="f8101-161">printCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="f8101-161">printCertificateSigningRequest</span></span>](../resources/printcertificatesigningrequest.md)|<span data-ttu-id="f8101-162">Запрос на подписание сертификата X.509 (CSR) для сертификата, созданного и используемой принтером для идентификации.</span><span class="sxs-lookup"><span data-stu-id="f8101-162">The X.509 Certificate Signing Request (CSR) for the certificate created and used by the printer to identify itself.</span></span>|<span data-ttu-id="f8101-163">Да</span><span class="sxs-lookup"><span data-stu-id="f8101-163">Yes</span></span>|
|<span data-ttu-id="f8101-164">connectorId</span><span class="sxs-lookup"><span data-stu-id="f8101-164">connectorId</span></span>|<span data-ttu-id="f8101-165">Строка</span><span class="sxs-lookup"><span data-stu-id="f8101-165">String</span></span>|<span data-ttu-id="f8101-166">ID соединителя, действующего в качестве прокси-сервера принтера.</span><span class="sxs-lookup"><span data-stu-id="f8101-166">ID of the connector acting as proxy to the printer.</span></span>|<span data-ttu-id="f8101-167">Нет</span><span class="sxs-lookup"><span data-stu-id="f8101-167">No</span></span>|

## <a name="response"></a><span data-ttu-id="f8101-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8101-168">Response</span></span>
<span data-ttu-id="f8101-169">В случае успешного использования этот метод возвращает код отклика и ссылку на связанный `202 Accepted` [принтерCreateOperation](../resources/printercreateoperation.md) в `Operation-Location` загонке.</span><span class="sxs-lookup"><span data-stu-id="f8101-169">If successful, this method returns a `202 Accepted` response code and a link to the associated [printerCreateOperation](../resources/printercreateoperation.md) in the `Operation-Location` header.</span></span>

<span data-ttu-id="f8101-170">Вы делаете запрос GET на связанный URL-адрес, чтобы получить состояние текущей регистрации принтера.</span><span class="sxs-lookup"><span data-stu-id="f8101-170">You make a GET request to the linked URL to get the status of an ongoing printer registration.</span></span> <span data-ttu-id="f8101-171">После успешного завершения регистрации принтера запрос GET на связанный URL-адрес будет содержать созданный объект принтера и зарегистрированный сертификат.</span><span class="sxs-lookup"><span data-stu-id="f8101-171">After printer registration has completed successfully, a GET request to the linked URL will contain the created printer object and registered certificate.</span></span>

## <a name="examples"></a><span data-ttu-id="f8101-172">Примеры</span><span class="sxs-lookup"><span data-stu-id="f8101-172">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f8101-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8101-173">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="f8101-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8101-174">Response</span></span>

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


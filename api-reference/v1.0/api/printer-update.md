---
title: Обновление принтера
description: Обновление свойств объекта принтера.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: e29335cab6d88c736825684b2ab46e65db64d563
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517386"
---
# <a name="update-printer"></a><span data-ttu-id="58787-103">Обновление принтера</span><span class="sxs-lookup"><span data-stu-id="58787-103">Update printer</span></span>
<span data-ttu-id="58787-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58787-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="58787-105">Обновление свойств объекта [принтера.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="58787-105">Update the properties of a [printer](../resources/printer.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="58787-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="58787-106">Permissions</span></span>
<span data-ttu-id="58787-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58787-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="58787-109">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="58787-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="58787-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="58787-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

><span data-ttu-id="58787-111">**Примечание:** Только приложение, которое зарегистрировал принтер, может обновлять принтер с помощью разрешений приложений.</span><span class="sxs-lookup"><span data-stu-id="58787-111">**Note:** Only the app that registered the printer is allowed to update the printer using application permissions.</span></span>

|<span data-ttu-id="58787-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58787-112">Permission type</span></span> | <span data-ttu-id="58787-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="58787-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="58787-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58787-114">Delegated (work or school account)</span></span>| <span data-ttu-id="58787-115">Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="58787-115">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="58787-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58787-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58787-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58787-117">Not Supported.</span></span>|
|<span data-ttu-id="58787-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="58787-118">Application</span></span>| <span data-ttu-id="58787-119">Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58787-119">Printer.ReadWrite.All</span></span> |

><span data-ttu-id="58787-120">**Примечание:** В настоящее время только принтеры, не оснащенные физическим устройством, могут обновляться с помощью разрешений приложений.</span><span class="sxs-lookup"><span data-stu-id="58787-120">**Note:** Right now, only printers that don't have physical device can be updated using application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="58787-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58787-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/printers/{printerId}
```

## <a name="request-headers"></a><span data-ttu-id="58787-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="58787-122">Request headers</span></span>
|<span data-ttu-id="58787-123">Имя</span><span class="sxs-lookup"><span data-stu-id="58787-123">Name</span></span>|<span data-ttu-id="58787-124">Описание</span><span class="sxs-lookup"><span data-stu-id="58787-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="58787-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="58787-125">Authorization</span></span>|<span data-ttu-id="58787-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58787-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="58787-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="58787-128">Content-Type</span></span>|<span data-ttu-id="58787-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58787-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="58787-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="58787-131">Request body</span></span>

### <a name="delegated-permissions-and-json-payload"></a><span data-ttu-id="58787-132">Делегирование разрешений и полезной нагрузки JSON</span><span class="sxs-lookup"><span data-stu-id="58787-132">Delegated permissions and JSON payload</span></span>

<span data-ttu-id="58787-133">При использовании делегирования разрешений в теле запроса поставляют значения для соответствующих полей принтера, которые необходимо обновить. [](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="58787-133">If using delegated permissions, in the request body, supply the values for the relevant [printer](../resources/printer.md) fields that should be updated.</span></span> <span data-ttu-id="58787-134">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="58787-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="58787-135">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="58787-135">For best performance, don't include existing values that haven't changed.</span></span> 

<span data-ttu-id="58787-136">Следующие свойства можно обновить с помощью делегирования разрешений.</span><span class="sxs-lookup"><span data-stu-id="58787-136">The following properties can be updated using delegated permissions.</span></span>

| <span data-ttu-id="58787-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="58787-137">Property</span></span>     | <span data-ttu-id="58787-138">Тип</span><span class="sxs-lookup"><span data-stu-id="58787-138">Type</span></span>        | <span data-ttu-id="58787-139">Описание</span><span class="sxs-lookup"><span data-stu-id="58787-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="58787-140">defaults</span><span class="sxs-lookup"><span data-stu-id="58787-140">defaults</span></span>|[<span data-ttu-id="58787-141">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="58787-141">printerDefaults</span></span>](../resources/printerdefaults.md)|<span data-ttu-id="58787-142">Параметры печати принтера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="58787-142">The printer's default print settings.</span></span>|
|<span data-ttu-id="58787-143">location</span><span class="sxs-lookup"><span data-stu-id="58787-143">location</span></span>|[<span data-ttu-id="58787-144">printerLocation</span><span class="sxs-lookup"><span data-stu-id="58787-144">printerLocation</span></span>](../resources/printerlocation.md)|<span data-ttu-id="58787-145">Физическое и/или организационное расположение принтера.</span><span class="sxs-lookup"><span data-stu-id="58787-145">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="58787-146">displayName</span><span class="sxs-lookup"><span data-stu-id="58787-146">displayName</span></span>|<span data-ttu-id="58787-147">Строка</span><span class="sxs-lookup"><span data-stu-id="58787-147">String</span></span>|<span data-ttu-id="58787-148">Имя принтера.</span><span class="sxs-lookup"><span data-stu-id="58787-148">The name of the printer.</span></span>|

### <a name="application-permissions-and-json-payload"></a><span data-ttu-id="58787-149">Разрешения приложения и полезной нагрузки JSON</span><span class="sxs-lookup"><span data-stu-id="58787-149">Application permissions and JSON payload</span></span>
<span data-ttu-id="58787-150">В теле запроса укажи значения [](../resources/printer.md) для соответствующих полей принтера, которые должны быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="58787-150">In the request body, supply the values for the relevant [printer](../resources/printer.md) fields that should be updated.</span></span> <span data-ttu-id="58787-151">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="58787-151">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="58787-152">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="58787-152">For best performance, don't include existing values that haven't changed.</span></span> 

<span data-ttu-id="58787-153">Следующие свойства можно обновить с помощью разрешений приложений.</span><span class="sxs-lookup"><span data-stu-id="58787-153">The following properties can be updated using application permissions.</span></span>

| <span data-ttu-id="58787-154">Свойство</span><span class="sxs-lookup"><span data-stu-id="58787-154">Property</span></span>     | <span data-ttu-id="58787-155">Тип</span><span class="sxs-lookup"><span data-stu-id="58787-155">Type</span></span>        | <span data-ttu-id="58787-156">Описание</span><span class="sxs-lookup"><span data-stu-id="58787-156">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="58787-157">defaults</span><span class="sxs-lookup"><span data-stu-id="58787-157">defaults</span></span>|[<span data-ttu-id="58787-158">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="58787-158">printerDefaults</span></span>](../resources/printerdefaults.md)|<span data-ttu-id="58787-159">Параметры печати принтера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="58787-159">The printer's default print settings.</span></span>|
|<span data-ttu-id="58787-160">capabilities</span><span class="sxs-lookup"><span data-stu-id="58787-160">capabilities</span></span>|[<span data-ttu-id="58787-161">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="58787-161">printerCapabilities</span></span>](../resources/printerCapabilities.md)|<span data-ttu-id="58787-162">Возможности принтера, связанного с этим разделом принтера.</span><span class="sxs-lookup"><span data-stu-id="58787-162">The capabilities of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="58787-163">displayName</span><span class="sxs-lookup"><span data-stu-id="58787-163">displayName</span></span>|<span data-ttu-id="58787-164">Строка</span><span class="sxs-lookup"><span data-stu-id="58787-164">String</span></span>|<span data-ttu-id="58787-165">Имя принтера.</span><span class="sxs-lookup"><span data-stu-id="58787-165">The name of the printer.</span></span>|
|<span data-ttu-id="58787-166">manufacturer</span><span class="sxs-lookup"><span data-stu-id="58787-166">manufacturer</span></span>|<span data-ttu-id="58787-167">String</span><span class="sxs-lookup"><span data-stu-id="58787-167">String</span></span>|<span data-ttu-id="58787-168">Производитель принтера.</span><span class="sxs-lookup"><span data-stu-id="58787-168">The manufacturer of the printer.</span></span>|
|<span data-ttu-id="58787-169">model</span><span class="sxs-lookup"><span data-stu-id="58787-169">model</span></span>|<span data-ttu-id="58787-170">String</span><span class="sxs-lookup"><span data-stu-id="58787-170">String</span></span>|<span data-ttu-id="58787-171">Имя модели принтера.</span><span class="sxs-lookup"><span data-stu-id="58787-171">The model name of the printer.</span></span>|
|<span data-ttu-id="58787-172">status</span><span class="sxs-lookup"><span data-stu-id="58787-172">status</span></span>|[<span data-ttu-id="58787-173">printerStatus</span><span class="sxs-lookup"><span data-stu-id="58787-173">printerStatus</span></span>](../resources/printerstatus.md)|<span data-ttu-id="58787-174">Состояние обработки принтера, включая ошибки.</span><span class="sxs-lookup"><span data-stu-id="58787-174">The processing status of the printer, including any errors.</span></span>|
|<span data-ttu-id="58787-175">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="58787-175">isAcceptingJobs</span></span>|<span data-ttu-id="58787-176">Логический</span><span class="sxs-lookup"><span data-stu-id="58787-176">Boolean</span></span>|<span data-ttu-id="58787-177">Принимает ли принтер новые задания печати.</span><span class="sxs-lookup"><span data-stu-id="58787-177">Whether the printer is currently accepting new print jobs.</span></span>|

### <a name="application-permissions-and-ipp-payload"></a><span data-ttu-id="58787-178">Разрешения приложений и полезной нагрузки IPP</span><span class="sxs-lookup"><span data-stu-id="58787-178">Application permissions and IPP payload</span></span>

<span data-ttu-id="58787-179">С разрешениями приложений принтер также может обновляться с помощью полезной нагрузки протокола интернет-печати (IPP).</span><span class="sxs-lookup"><span data-stu-id="58787-179">With application permissions, a printer can also be updated using an Internet Printing Protocol (IPP) payload.</span></span> <span data-ttu-id="58787-180">В этом случае тело запроса содержит двоичный поток, представляюющий группу атрибутов принтера в [кодовом коде IPP.](https://tools.ietf.org/html/rfc8010)</span><span class="sxs-lookup"><span data-stu-id="58787-180">In this case, the request body contains a binary stream that represents the Printer Attributes group in [IPP encoding](https://tools.ietf.org/html/rfc8010).</span></span>

<span data-ttu-id="58787-181">Клиент должен предоставить набор атрибутов принтера с одним или более значениями (включая явно разрешенные вне диапазона значения), как это определено в разделе [RFC8011 раздела 5.2](https://tools.ietf.org/html/rfc8011#section-5.2) Атрибуты шаблона работы ("xxx-default", "xxx-supported" и "xxx-ready"), Атрибуты описания принтера [5.4](https://tools.ietf.org/html/rfc8011#section-5.4) и все расширения атрибутов, поддерживаемые принтером.</span><span class="sxs-lookup"><span data-stu-id="58787-181">The client MUST supply a set of Printer attributes with one or more values (including explicitly allowed out-of-band values) as defined in [RFC8011 section 5.2](https://tools.ietf.org/html/rfc8011#section-5.2) Job Template Attributes ("xxx-default", "xxx-supported", and "xxx-ready" attributes), [Section 5.4](https://tools.ietf.org/html/rfc8011#section-5.4) Printer Description Attributes, and any attribute extensions supported by the Printer.</span></span> <span data-ttu-id="58787-182">Значение (ы) каждого предоставленного атрибута принтера заменяет значение (ы) соответствующего атрибута принтера на объекте целевого принтера.</span><span class="sxs-lookup"><span data-stu-id="58787-182">The value(s) of each Printer attribute supplied replaces the value(s) of the corresponding Printer attribute on the target Printer object.</span></span> <span data-ttu-id="58787-183">Для атрибутов, которые могут иметь несколько значений (1setOf), все значения, предоставленные клиентом, заменяют все значения соответствующего атрибута объекта Printer.</span><span class="sxs-lookup"><span data-stu-id="58787-183">For attributes that can have multiple values (1setOf), all values supplied by the client replace all values of the corresponding Printer object attribute.</span></span>

## <a name="response"></a><span data-ttu-id="58787-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="58787-184">Response</span></span>

### <a name="delegated-permissions-and-json-payload"></a><span data-ttu-id="58787-185">Делегирование разрешений и полезной нагрузки JSON</span><span class="sxs-lookup"><span data-stu-id="58787-185">Delegated permissions and JSON payload</span></span>

<span data-ttu-id="58787-186">При использовании делегирования разрешений при успешном использовании этот метод возвращает код отклика и обновленный объект принтера `200 OK` в тексте [](../resources/printer.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="58787-186">If using delegated permissions, if successful, this method returns a `200 OK` response code and an updated [printer](../resources/printer.md) object in the response body.</span></span>

### <a name="application-permissions-and-json-payload"></a><span data-ttu-id="58787-187">Разрешения приложения и полезной нагрузки JSON</span><span class="sxs-lookup"><span data-stu-id="58787-187">Application permissions and JSON payload</span></span>

<span data-ttu-id="58787-188">При использовании делегирования разрешений при успешном использовании этот метод возвращает код отклика и обновленный объект принтера `200 OK` в тексте [](../resources/printer.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="58787-188">If using delegated permissions, if successful, this method returns a `200 OK` response code and an updated [printer](../resources/printer.md) object in the response body.</span></span>

### <a name="application-permissions-and-ipp-payload"></a><span data-ttu-id="58787-189">Разрешения приложений и полезной нагрузки IPP</span><span class="sxs-lookup"><span data-stu-id="58787-189">Application permissions and IPP payload</span></span>

<span data-ttu-id="58787-190">При использовании разрешений приложений при успешном использовании этот метод возвращает `204 No content` код ответа.</span><span class="sxs-lookup"><span data-stu-id="58787-190">If using application permissions, if successful, this method returns `204 No content` response code.</span></span> <span data-ttu-id="58787-191">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="58787-191">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="58787-192">Примеры</span><span class="sxs-lookup"><span data-stu-id="58787-192">Examples</span></span>

### <a name="request"></a><span data-ttu-id="58787-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="58787-193">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_printer"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/print/printers/{printerId}
Content-Type: application/json
Content-length: 581

{
  "name": "PrinterName",
  "location": {
    "latitude": 1.1,
    "longitude": 2.2,
    "altitudeInMeters": 3
  }
}
```


### <a name="response"></a><span data-ttu-id="58787-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="58787-194">Response</span></span>
<span data-ttu-id="58787-195">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="58787-195">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printer"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers/$entity",
  "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
  "displayName": "PrinterName",
  "manufacturer": "PrinterManufacturer",
  "model": "PrinterModel",
  "isShared": true,
  "registeredDateTime": "2020-02-04T00:00:00.0000000Z",
  "isAcceptingJobs": true,
  "status": {
    "state": "idle",
    "details": [],
    "description": ""
  },
  "defaults": {
    "copiesPerJob":1,
    "contentType": "application/oxps",
    "finishings": ["none"],
    "mediaType": "stationery"
  },
  "location": {
    "latitude": 1.1,
    "longitude": 2.2,
    "altitudeInMeters": 3,
    "streetAddress": "One Microsoft Way",
    "subUnit": [
        "Main Plaza",
        "Unit 400"
    ],
    "city": "Redmond",
    "postalCode": "98052",
    "countryOrRegion": "USA",
    "site": "Puget Sound",
    "building": "Studio E",
    "floor": "1",
    "floorDescription": "First Floor",
    "roomName": "1234",
    "roomDescription": "First floor copy room",
    "organization": [
        "C+AI",
        "Microsoft Graph"
    ],
    "subdivision": [
        "King County",
        "Red West"
    ],
    "stateOrProvince": "Washington"
  }
}
```


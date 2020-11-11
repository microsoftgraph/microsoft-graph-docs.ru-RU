---
title: Обновление принтера
description: Обновление свойств объекта Printer.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 95af5526edbbd40a65e3356efa7cee76cf135c14
ms.sourcegitcommit: a9720ab80625a4692f7d2450164717853535d0b0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/11/2020
ms.locfileid: "48993980"
---
# <a name="update-printer"></a><span data-ttu-id="5b4f2-103">Обновление принтера</span><span class="sxs-lookup"><span data-stu-id="5b4f2-103">Update printer</span></span>

<span data-ttu-id="5b4f2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b4f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b4f2-105">Обновление свойств объекта [Printer](../resources/printer.md) .</span><span class="sxs-lookup"><span data-stu-id="5b4f2-105">Update the properties of a [printer](../resources/printer.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b4f2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5b4f2-106">Permissions</span></span>
<span data-ttu-id="5b4f2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b4f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="5b4f2-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="5b4f2-110">Пользователь, вошедшего в систему, должен быть [администратором принтера](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="5b4f2-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

<span data-ttu-id="5b4f2-111">Только приложение, которое зарегистрировало принтер, может обновлять принтер с помощью разрешений приложения.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-111">Only the app that registered the printer is allowed to update the printer using application permissions.</span></span>

|<span data-ttu-id="5b4f2-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b4f2-112">Permission type</span></span> | <span data-ttu-id="5b4f2-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b4f2-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="5b4f2-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b4f2-114">Delegated (work or school account)</span></span>| <span data-ttu-id="5b4f2-115">Printer. ReadWrite. ALL, Printer. FullControl. ALL</span><span class="sxs-lookup"><span data-stu-id="5b4f2-115">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="5b4f2-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b4f2-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b4f2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-117">Not Supported.</span></span>|
|<span data-ttu-id="5b4f2-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="5b4f2-118">Application</span></span>| <span data-ttu-id="5b4f2-119">Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b4f2-119">Printer.ReadWrite.All</span></span> |

><span data-ttu-id="5b4f2-120">**Примечание:** Сейчас только принтеры, на которых не установлено физическое устройство, могут обновляться с помощью разрешений приложения.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-120">**Note:** Right now, only printers that don't have physical device can be updated using application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="5b4f2-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b4f2-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/printers/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5b4f2-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b4f2-122">Request headers</span></span>
| <span data-ttu-id="5b4f2-123">Имя</span><span class="sxs-lookup"><span data-stu-id="5b4f2-123">Name</span></span>       | <span data-ttu-id="5b4f2-124">Описание</span><span class="sxs-lookup"><span data-stu-id="5b4f2-124">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5b4f2-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5b4f2-125">Authorization</span></span> | <span data-ttu-id="5b4f2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5b4f2-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5b4f2-128">Content-type</span></span>  | <span data-ttu-id="5b4f2-129">`application/json` При использовании делегированных разрешений `application/ipp` при использовании разрешений приложения.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-129">`application/json` when using delegated permissions, `application/ipp` when using application permissions.</span></span> <span data-ttu-id="5b4f2-130">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-130">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b4f2-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b4f2-131">Request body</span></span>

### <a name="delegated-permissions-and-json-payload"></a><span data-ttu-id="5b4f2-132">Делегированные разрешения и полезные данные JSON</span><span class="sxs-lookup"><span data-stu-id="5b4f2-132">Delegated permissions and JSON payload</span></span>

<span data-ttu-id="5b4f2-133">Если в тексте запроса используется делегированные разрешения, укажите значения для соответствующих полей [принтера](../resources/printer.md) , которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-133">If using delegated permissions, in the request body, supply the values for the relevant [printer](../resources/printer.md) fields that should be updated.</span></span> <span data-ttu-id="5b4f2-134">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5b4f2-135">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-135">For best performance, don't include existing values that haven't changed.</span></span> 

<span data-ttu-id="5b4f2-136">Следующие свойства можно обновлять с делегированными разрешениями.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-136">The following properties can be updated using delegated permissions.</span></span>

| <span data-ttu-id="5b4f2-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b4f2-137">Property</span></span>     | <span data-ttu-id="5b4f2-138">Тип</span><span class="sxs-lookup"><span data-stu-id="5b4f2-138">Type</span></span>        | <span data-ttu-id="5b4f2-139">Описание</span><span class="sxs-lookup"><span data-stu-id="5b4f2-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5b4f2-140">defaults</span><span class="sxs-lookup"><span data-stu-id="5b4f2-140">defaults</span></span>|[<span data-ttu-id="5b4f2-141">принтердефаултс</span><span class="sxs-lookup"><span data-stu-id="5b4f2-141">printerDefaults</span></span>](../resources/printerdefaults.md)|<span data-ttu-id="5b4f2-142">Параметры печати по умолчанию для принтера.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-142">The printer's default print settings.</span></span>|
|<span data-ttu-id="5b4f2-143">расположение</span><span class="sxs-lookup"><span data-stu-id="5b4f2-143">location</span></span>|[<span data-ttu-id="5b4f2-144">принтерлокатион</span><span class="sxs-lookup"><span data-stu-id="5b4f2-144">printerLocation</span></span>](../resources/printerlocation.md)|<span data-ttu-id="5b4f2-145">Физическое и/или организационное расположение принтера.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-145">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="5b4f2-146">displayName</span><span class="sxs-lookup"><span data-stu-id="5b4f2-146">displayName</span></span>|<span data-ttu-id="5b4f2-147">String</span><span class="sxs-lookup"><span data-stu-id="5b4f2-147">String</span></span>|<span data-ttu-id="5b4f2-148">Имя принтера.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-148">The name of the printer.</span></span>|

### <a name="application-permissions-and-json-payload"></a><span data-ttu-id="5b4f2-149">Разрешения приложений и полезные данные JSON</span><span class="sxs-lookup"><span data-stu-id="5b4f2-149">Application permissions and JSON payload</span></span>
<span data-ttu-id="5b4f2-150">В тексте запроса укажите значения для соответствующих полей [принтера](../resources/printer.md) , которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-150">In the request body, supply the values for the relevant [printer](../resources/printer.md) fields that should be updated.</span></span> <span data-ttu-id="5b4f2-151">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-151">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5b4f2-152">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-152">For best performance, don't include existing values that haven't changed.</span></span> 

<span data-ttu-id="5b4f2-153">Следующие свойства можно обновлять с помощью разрешений приложения.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-153">The following properties can be updated using application permissions.</span></span>

| <span data-ttu-id="5b4f2-154">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b4f2-154">Property</span></span>     | <span data-ttu-id="5b4f2-155">Тип</span><span class="sxs-lookup"><span data-stu-id="5b4f2-155">Type</span></span>        | <span data-ttu-id="5b4f2-156">Описание</span><span class="sxs-lookup"><span data-stu-id="5b4f2-156">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5b4f2-157">defaults</span><span class="sxs-lookup"><span data-stu-id="5b4f2-157">defaults</span></span>|[<span data-ttu-id="5b4f2-158">принтердефаултс</span><span class="sxs-lookup"><span data-stu-id="5b4f2-158">printerDefaults</span></span>](../resources/printerdefaults.md)|<span data-ttu-id="5b4f2-159">Параметры печати по умолчанию для принтера.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-159">The printer's default print settings.</span></span>|
|<span data-ttu-id="5b4f2-160">capabilities</span><span class="sxs-lookup"><span data-stu-id="5b4f2-160">capabilities</span></span>|[<span data-ttu-id="5b4f2-161">принтеркапабилитиес</span><span class="sxs-lookup"><span data-stu-id="5b4f2-161">printerCapabilities</span></span>](../resources/printerCapabilities.md)|<span data-ttu-id="5b4f2-162">Возможности принтера, связанного с этим общим принтером.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-162">The capabilities of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="5b4f2-163">displayName</span><span class="sxs-lookup"><span data-stu-id="5b4f2-163">displayName</span></span>|<span data-ttu-id="5b4f2-164">String</span><span class="sxs-lookup"><span data-stu-id="5b4f2-164">String</span></span>|<span data-ttu-id="5b4f2-165">Имя принтера.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-165">The name of the printer.</span></span>|
|<span data-ttu-id="5b4f2-166">manufacturer</span><span class="sxs-lookup"><span data-stu-id="5b4f2-166">manufacturer</span></span>|<span data-ttu-id="5b4f2-167">String</span><span class="sxs-lookup"><span data-stu-id="5b4f2-167">String</span></span>|<span data-ttu-id="5b4f2-168">Производитель принтера.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-168">The manufacturer of the printer.</span></span>|
|<span data-ttu-id="5b4f2-169">model</span><span class="sxs-lookup"><span data-stu-id="5b4f2-169">model</span></span>|<span data-ttu-id="5b4f2-170">String</span><span class="sxs-lookup"><span data-stu-id="5b4f2-170">String</span></span>|<span data-ttu-id="5b4f2-171">Имя модели принтера.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-171">The model name of the printer.</span></span>|
|<span data-ttu-id="5b4f2-172">status</span><span class="sxs-lookup"><span data-stu-id="5b4f2-172">status</span></span>|[<span data-ttu-id="5b4f2-173">принтерстатус</span><span class="sxs-lookup"><span data-stu-id="5b4f2-173">printerStatus</span></span>](../resources/printerstatus.md)|<span data-ttu-id="5b4f2-174">Состояние обработки принтера, включая ошибки.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-174">The processing status of the printer, including any errors.</span></span>|
|<span data-ttu-id="5b4f2-175">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="5b4f2-175">isAcceptingJobs</span></span>|<span data-ttu-id="5b4f2-176">Логический</span><span class="sxs-lookup"><span data-stu-id="5b4f2-176">Boolean</span></span>|<span data-ttu-id="5b4f2-177">Принимает ли принтер новые задания печати.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-177">Whether the printer is currently accepting new print jobs.</span></span>|

### <a name="application-permissions-and-ipp-payload"></a><span data-ttu-id="5b4f2-178">Разрешения приложений и полезные данные IPP</span><span class="sxs-lookup"><span data-stu-id="5b4f2-178">Application permissions and IPP payload</span></span>

<span data-ttu-id="5b4f2-179">С разрешениями приложения принтер также может обновляться с помощью полезных данных протокола Internet Printing Protocol (IPP).</span><span class="sxs-lookup"><span data-stu-id="5b4f2-179">With application permissions, a printer can also be updated using an Internet Printing Protocol (IPP) payload.</span></span> <span data-ttu-id="5b4f2-180">В этом случае текст запроса содержит двоичный поток, представляющий группу атрибутов принтера в [кодировке IPP](https://tools.ietf.org/html/rfc8010).</span><span class="sxs-lookup"><span data-stu-id="5b4f2-180">In this case, the request body contains a binary stream that represents the Printer Attributes group in [IPP encoding](https://tools.ietf.org/html/rfc8010).</span></span>

<span data-ttu-id="5b4f2-181">Клиент должен предоставить набор атрибутов принтера с одним или несколькими значениями (включая явно разрешенные значения из диапазона), как определено в [разделе RFC8011 section 5,2](https://tools.ietf.org/html/rfc8011#section-5.2) атрибуты шаблона задания ("XXX-Default", "XXX-supported" и "XXX-Ready"), [Section 5,4](https://tools.ietf.org/html/rfc8011#section-5.4) атрибуты описания принтера и все расширения атрибутов, поддерживаемые принтером.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-181">The client MUST supply a set of Printer attributes with one or more values (including explicitly allowed out-of-band values) as defined in [RFC8011 section 5.2](https://tools.ietf.org/html/rfc8011#section-5.2) Job Template Attributes ("xxx-default", "xxx-supported", and "xxx-ready" attributes), [Section 5.4](https://tools.ietf.org/html/rfc8011#section-5.4) Printer Description Attributes, and any attribute extensions supported by the Printer.</span></span> <span data-ttu-id="5b4f2-182">Значения каждого из указанных атрибутов принтера заменяют значения соответствующего атрибута принтера для целевого объекта Printer.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-182">The value(s) of each Printer attribute supplied replaces the value(s) of the corresponding Printer attribute on the target Printer object.</span></span> <span data-ttu-id="5b4f2-183">Для атрибутов, которые могут иметь несколько значений (1setOf), все значения, предоставляемые клиентом, заменяют все значения атрибута соответствующего объекта Printer.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-183">For attributes that can have multiple values (1setOf), all values supplied by the client replace all values of the corresponding Printer object attribute.</span></span>

## <a name="response"></a><span data-ttu-id="5b4f2-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b4f2-184">Response</span></span>

### <a name="delegated-permissions-and-json-payload"></a><span data-ttu-id="5b4f2-185">Делегированные разрешения и полезные данные JSON</span><span class="sxs-lookup"><span data-stu-id="5b4f2-185">Delegated permissions and JSON payload</span></span>

<span data-ttu-id="5b4f2-186">При успешном использовании делегированных разрешений этот метод возвращает `200 OK` код отклика и обновленный объект [Printer](../resources/printer.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-186">If using delegated permissions, if successful, this method returns a `200 OK` response code and an updated [printer](../resources/printer.md) object in the response body.</span></span>

### <a name="application-permissions-and-json-payload"></a><span data-ttu-id="5b4f2-187">Разрешения приложений и полезные данные JSON</span><span class="sxs-lookup"><span data-stu-id="5b4f2-187">Application permissions and JSON payload</span></span>

<span data-ttu-id="5b4f2-188">При успешном использовании делегированных разрешений этот метод возвращает `200 OK` код отклика и обновленный объект [Printer](../resources/printer.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-188">If using delegated permissions, if successful, this method returns a `200 OK` response code and an updated [printer](../resources/printer.md) object in the response body.</span></span>

### <a name="application-permissions-and-ipp-payload"></a><span data-ttu-id="5b4f2-189">Разрешения приложений и полезные данные IPP</span><span class="sxs-lookup"><span data-stu-id="5b4f2-189">Application permissions and IPP payload</span></span>

<span data-ttu-id="5b4f2-190">Если при успешном использовании разрешений приложения этот метод возвращает `204 No content` код отклика.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-190">If using application permissions, if successful, this method returns `204 No content` response code.</span></span> <span data-ttu-id="5b4f2-191">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-191">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b4f2-192">Пример</span><span class="sxs-lookup"><span data-stu-id="5b4f2-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b4f2-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b4f2-193">Request</span></span>
<span data-ttu-id="5b4f2-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-194">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5b4f2-195">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b4f2-195">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_printer"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/printers/{id}
Content-type: application/json
Content-length: 124

{
  "name": "PrinterName",
  "location": {
    "latitude": 1.1,
    "longitude": 2.2,
    "altitudeInMeters": 3
  }
}
```
# <a name="c"></a>[<span data-ttu-id="5b4f2-196">C#</span><span class="sxs-lookup"><span data-stu-id="5b4f2-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5b4f2-197">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b4f2-197">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5b4f2-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b4f2-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5b4f2-199">Java</span><span class="sxs-lookup"><span data-stu-id="5b4f2-199">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-printer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="5b4f2-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b4f2-200">Response</span></span>
<span data-ttu-id="5b4f2-201">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-201">The following is an example of the response.</span></span>
><span data-ttu-id="5b4f2-p110">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b4f2-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printer"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1313

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers/$entity",
  "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
  "name": "PrinterName",
  "manufacturer": "PrinterManufacturer",
  "model": "PrinterModel",
  "isShared": true,
  "registeredDateTime": "2020-02-04T00:00:00.0000000Z",
  "acceptingJobs": true,
  "status": {
    "processingState": "idle",
    "processingStateReasons": [],
    "processingStateDescription": ""
  },
  "defaults": {
    "copiesPerJob":1,
    "documentMimeType": "application/oxps",
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
    "floorNumber": 1,
    "floorDescription": "First Floor",
    "roomNumber": 1234,
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update printer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

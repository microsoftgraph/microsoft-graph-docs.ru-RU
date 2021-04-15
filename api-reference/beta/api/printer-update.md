---
title: Обновление принтера
description: Обновление свойств объекта принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 2a0d40490365a2974a83683f7b9564063f8e25c0
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766226"
---
# <a name="update-printer"></a><span data-ttu-id="04d7b-103">Обновление принтера</span><span class="sxs-lookup"><span data-stu-id="04d7b-103">Update printer</span></span>

<span data-ttu-id="04d7b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04d7b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04d7b-105">Обновление свойств объекта [принтера.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="04d7b-105">Update the properties of a [printer](../resources/printer.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="04d7b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04d7b-106">Permissions</span></span>
<span data-ttu-id="04d7b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04d7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="04d7b-109">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="04d7b-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="04d7b-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="04d7b-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

<span data-ttu-id="04d7b-111">Только приложение, которое зарегистрировал принтер, может обновлять принтер с помощью разрешений приложений.</span><span class="sxs-lookup"><span data-stu-id="04d7b-111">Only the app that registered the printer is allowed to update the printer using application permissions.</span></span>

|<span data-ttu-id="04d7b-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04d7b-112">Permission type</span></span> | <span data-ttu-id="04d7b-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="04d7b-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="04d7b-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04d7b-114">Delegated (work or school account)</span></span>| <span data-ttu-id="04d7b-115">Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="04d7b-115">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="04d7b-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04d7b-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04d7b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04d7b-117">Not Supported.</span></span>|
|<span data-ttu-id="04d7b-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="04d7b-118">Application</span></span>| <span data-ttu-id="04d7b-119">Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04d7b-119">Printer.ReadWrite.All</span></span> |

><span data-ttu-id="04d7b-120">**Примечание:** В настоящее время только принтеры, не оснащенные физическим устройством, могут обновляться с помощью разрешений приложений.</span><span class="sxs-lookup"><span data-stu-id="04d7b-120">**Note:** Right now, only printers that don't have physical device can be updated using application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="04d7b-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04d7b-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/printers/{id}
```
## <a name="request-headers"></a><span data-ttu-id="04d7b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04d7b-122">Request headers</span></span>
| <span data-ttu-id="04d7b-123">Имя</span><span class="sxs-lookup"><span data-stu-id="04d7b-123">Name</span></span>       | <span data-ttu-id="04d7b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="04d7b-124">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="04d7b-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04d7b-125">Authorization</span></span> | <span data-ttu-id="04d7b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04d7b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="04d7b-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="04d7b-128">Content-type</span></span>  | <span data-ttu-id="04d7b-129">`application/json` при использовании делегирования разрешений или `application/ipp` `application/json` при использовании разрешений приложений.</span><span class="sxs-lookup"><span data-stu-id="04d7b-129">`application/json` when using delegated permissions, `application/ipp` or `application/json` when using application permissions.</span></span> <span data-ttu-id="04d7b-130">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="04d7b-130">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="04d7b-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04d7b-131">Request body</span></span>

### <a name="delegated-permissions-and-json-payload"></a><span data-ttu-id="04d7b-132">Делегирование разрешений и полезной нагрузки JSON</span><span class="sxs-lookup"><span data-stu-id="04d7b-132">Delegated permissions and JSON payload</span></span>

<span data-ttu-id="04d7b-133">При использовании делегирования разрешений в теле запроса поставляют значения для соответствующих полей принтера, которые необходимо обновить. [](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="04d7b-133">If using delegated permissions, in the request body, supply the values for the relevant [printer](../resources/printer.md) fields that should be updated.</span></span> <span data-ttu-id="04d7b-134">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="04d7b-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="04d7b-135">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="04d7b-135">For best performance, don't include existing values that haven't changed.</span></span> 

<span data-ttu-id="04d7b-136">Следующие свойства можно обновить с помощью делегирования разрешений.</span><span class="sxs-lookup"><span data-stu-id="04d7b-136">The following properties can be updated using delegated permissions.</span></span>

| <span data-ttu-id="04d7b-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="04d7b-137">Property</span></span>     | <span data-ttu-id="04d7b-138">Тип</span><span class="sxs-lookup"><span data-stu-id="04d7b-138">Type</span></span>        | <span data-ttu-id="04d7b-139">Описание</span><span class="sxs-lookup"><span data-stu-id="04d7b-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="04d7b-140">defaults</span><span class="sxs-lookup"><span data-stu-id="04d7b-140">defaults</span></span>|[<span data-ttu-id="04d7b-141">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="04d7b-141">printerDefaults</span></span>](../resources/printerdefaults.md)|<span data-ttu-id="04d7b-142">Параметры печати принтера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="04d7b-142">The printer's default print settings.</span></span>|
|<span data-ttu-id="04d7b-143">расположение</span><span class="sxs-lookup"><span data-stu-id="04d7b-143">location</span></span>|[<span data-ttu-id="04d7b-144">printerLocation</span><span class="sxs-lookup"><span data-stu-id="04d7b-144">printerLocation</span></span>](../resources/printerlocation.md)|<span data-ttu-id="04d7b-145">Физическое и/или организационное расположение принтера.</span><span class="sxs-lookup"><span data-stu-id="04d7b-145">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="04d7b-146">displayName</span><span class="sxs-lookup"><span data-stu-id="04d7b-146">displayName</span></span>|<span data-ttu-id="04d7b-147">String</span><span class="sxs-lookup"><span data-stu-id="04d7b-147">String</span></span>|<span data-ttu-id="04d7b-148">Имя принтера.</span><span class="sxs-lookup"><span data-stu-id="04d7b-148">The name of the printer.</span></span>|

### <a name="application-permissions-and-json-payload"></a><span data-ttu-id="04d7b-149">Разрешения приложения и полезной нагрузки JSON</span><span class="sxs-lookup"><span data-stu-id="04d7b-149">Application permissions and JSON payload</span></span>
<span data-ttu-id="04d7b-150">В теле запроса укажи значения [](../resources/printer.md) для соответствующих полей принтера, которые должны быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="04d7b-150">In the request body, supply the values for the relevant [printer](../resources/printer.md) fields that should be updated.</span></span> <span data-ttu-id="04d7b-151">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="04d7b-151">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="04d7b-152">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="04d7b-152">For best performance, don't include existing values that haven't changed.</span></span> 

<span data-ttu-id="04d7b-153">Следующие свойства можно обновить с помощью разрешений приложений.</span><span class="sxs-lookup"><span data-stu-id="04d7b-153">The following properties can be updated using application permissions.</span></span>

| <span data-ttu-id="04d7b-154">Свойство</span><span class="sxs-lookup"><span data-stu-id="04d7b-154">Property</span></span>     | <span data-ttu-id="04d7b-155">Тип</span><span class="sxs-lookup"><span data-stu-id="04d7b-155">Type</span></span>        | <span data-ttu-id="04d7b-156">Описание</span><span class="sxs-lookup"><span data-stu-id="04d7b-156">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="04d7b-157">defaults</span><span class="sxs-lookup"><span data-stu-id="04d7b-157">defaults</span></span>|[<span data-ttu-id="04d7b-158">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="04d7b-158">printerDefaults</span></span>](../resources/printerdefaults.md)|<span data-ttu-id="04d7b-159">Параметры печати принтера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="04d7b-159">The printer's default print settings.</span></span>|
|<span data-ttu-id="04d7b-160">capabilities</span><span class="sxs-lookup"><span data-stu-id="04d7b-160">capabilities</span></span>|[<span data-ttu-id="04d7b-161">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="04d7b-161">printerCapabilities</span></span>](../resources/printerCapabilities.md)|<span data-ttu-id="04d7b-162">Возможности принтера, связанного с этим разделом принтера.</span><span class="sxs-lookup"><span data-stu-id="04d7b-162">The capabilities of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="04d7b-163">displayName</span><span class="sxs-lookup"><span data-stu-id="04d7b-163">displayName</span></span>|<span data-ttu-id="04d7b-164">String</span><span class="sxs-lookup"><span data-stu-id="04d7b-164">String</span></span>|<span data-ttu-id="04d7b-165">Имя принтера.</span><span class="sxs-lookup"><span data-stu-id="04d7b-165">The name of the printer.</span></span>|
|<span data-ttu-id="04d7b-166">manufacturer</span><span class="sxs-lookup"><span data-stu-id="04d7b-166">manufacturer</span></span>|<span data-ttu-id="04d7b-167">String</span><span class="sxs-lookup"><span data-stu-id="04d7b-167">String</span></span>|<span data-ttu-id="04d7b-168">Производитель принтера.</span><span class="sxs-lookup"><span data-stu-id="04d7b-168">The manufacturer of the printer.</span></span>|
|<span data-ttu-id="04d7b-169">model</span><span class="sxs-lookup"><span data-stu-id="04d7b-169">model</span></span>|<span data-ttu-id="04d7b-170">String</span><span class="sxs-lookup"><span data-stu-id="04d7b-170">String</span></span>|<span data-ttu-id="04d7b-171">Имя модели принтера.</span><span class="sxs-lookup"><span data-stu-id="04d7b-171">The model name of the printer.</span></span>|
|<span data-ttu-id="04d7b-172">status</span><span class="sxs-lookup"><span data-stu-id="04d7b-172">status</span></span>|[<span data-ttu-id="04d7b-173">printerStatus</span><span class="sxs-lookup"><span data-stu-id="04d7b-173">printerStatus</span></span>](../resources/printerstatus.md)|<span data-ttu-id="04d7b-174">Состояние обработки принтера, включая ошибки.</span><span class="sxs-lookup"><span data-stu-id="04d7b-174">The processing status of the printer, including any errors.</span></span>|
|<span data-ttu-id="04d7b-175">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="04d7b-175">isAcceptingJobs</span></span>|<span data-ttu-id="04d7b-176">Логический</span><span class="sxs-lookup"><span data-stu-id="04d7b-176">Boolean</span></span>|<span data-ttu-id="04d7b-177">Принимает ли принтер новые задания печати.</span><span class="sxs-lookup"><span data-stu-id="04d7b-177">Whether the printer is currently accepting new print jobs.</span></span>|

### <a name="application-permissions-and-ipp-payload"></a><span data-ttu-id="04d7b-178">Разрешения приложений и полезной нагрузки IPP</span><span class="sxs-lookup"><span data-stu-id="04d7b-178">Application permissions and IPP payload</span></span>

<span data-ttu-id="04d7b-179">С разрешениями приложений принтер также может обновляться с помощью полезной нагрузки протокола интернет-печати (IPP).</span><span class="sxs-lookup"><span data-stu-id="04d7b-179">With application permissions, a printer can also be updated using an Internet Printing Protocol (IPP) payload.</span></span> <span data-ttu-id="04d7b-180">В этом случае тело запроса содержит двоичный поток, представляюющий группу атрибутов принтера в [кодовом коде IPP.](https://tools.ietf.org/html/rfc8010)</span><span class="sxs-lookup"><span data-stu-id="04d7b-180">In this case, the request body contains a binary stream that represents the Printer Attributes group in [IPP encoding](https://tools.ietf.org/html/rfc8010).</span></span>

<span data-ttu-id="04d7b-181">Клиент должен предоставить набор атрибутов принтера с одним или более значениями (включая явно разрешенные вне диапазона значения), как это определено в разделе [RFC8011 раздела 5.2](https://tools.ietf.org/html/rfc8011#section-5.2) Атрибуты шаблона работы ("xxx-default", "xxx-supported" и "xxx-ready"), Атрибуты описания принтера [5.4](https://tools.ietf.org/html/rfc8011#section-5.4) и все расширения атрибутов, поддерживаемые принтером.</span><span class="sxs-lookup"><span data-stu-id="04d7b-181">The client MUST supply a set of Printer attributes with one or more values (including explicitly allowed out-of-band values) as defined in [RFC8011 section 5.2](https://tools.ietf.org/html/rfc8011#section-5.2) Job Template Attributes ("xxx-default", "xxx-supported", and "xxx-ready" attributes), [Section 5.4](https://tools.ietf.org/html/rfc8011#section-5.4) Printer Description Attributes, and any attribute extensions supported by the Printer.</span></span> <span data-ttu-id="04d7b-182">Значение (ы) каждого предоставленного атрибута принтера заменяет значение (ы) соответствующего атрибута принтера на объекте целевого принтера.</span><span class="sxs-lookup"><span data-stu-id="04d7b-182">The value(s) of each Printer attribute supplied replaces the value(s) of the corresponding Printer attribute on the target Printer object.</span></span> <span data-ttu-id="04d7b-183">Для атрибутов, которые могут иметь несколько значений (1setOf), все значения, предоставленные клиентом, заменяют все значения соответствующего атрибута объекта Printer.</span><span class="sxs-lookup"><span data-stu-id="04d7b-183">For attributes that can have multiple values (1setOf), all values supplied by the client replace all values of the corresponding Printer object attribute.</span></span>

> <span data-ttu-id="04d7b-184">**Примечание:** Не пропускать атрибуты операции в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="04d7b-184">**Note:** Do not pass operation attributes in the request body.</span></span> <span data-ttu-id="04d7b-185">Тело запроса должно содержать только атрибуты принтера.</span><span class="sxs-lookup"><span data-stu-id="04d7b-185">The request body should only contain printer attributes.</span></span>


> <span data-ttu-id="04d7b-186">**Примечание:** Чтобы принтеры работали с определенной платформой, она должна соответствовать требованиям этой платформы.</span><span class="sxs-lookup"><span data-stu-id="04d7b-186">**Note:** For printers to work with a particular platform, it should meet the requirements of that platform.</span></span> <span data-ttu-id="04d7b-187">Например, на клиенте Windows ожидается, что принтер указывает все атрибуты, которые считаются обязательными в спецификациях [MOPRIA.](https://mopria.org)</span><span class="sxs-lookup"><span data-stu-id="04d7b-187">For example, on windows client, it is expected that printer specifies all attributes that are considered mandatory as per [MOPRIA](https://mopria.org) specs.</span></span> <span data-ttu-id="04d7b-188">Обратите внимание, что спецификации MOPRIA доступны только платным членам MOPRIA.</span><span class="sxs-lookup"><span data-stu-id="04d7b-188">Please note MOPRIA specs are available to only the paid members of MOPRIA.</span></span>

## <a name="response"></a><span data-ttu-id="04d7b-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="04d7b-189">Response</span></span>

### <a name="delegated-permissions-and-json-payload"></a><span data-ttu-id="04d7b-190">Делегирование разрешений и полезной нагрузки JSON</span><span class="sxs-lookup"><span data-stu-id="04d7b-190">Delegated permissions and JSON payload</span></span>

<span data-ttu-id="04d7b-191">При использовании делегирования разрешений при успешном использовании этот метод возвращает код отклика и обновленный объект принтера `200 OK` в тексте [](../resources/printer.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="04d7b-191">If using delegated permissions, if successful, this method returns a `200 OK` response code and an updated [printer](../resources/printer.md) object in the response body.</span></span>

### <a name="application-permissions-and-json-payload"></a><span data-ttu-id="04d7b-192">Разрешения приложения и полезной нагрузки JSON</span><span class="sxs-lookup"><span data-stu-id="04d7b-192">Application permissions and JSON payload</span></span>

<span data-ttu-id="04d7b-193">При использовании делегирования разрешений при успешном использовании этот метод возвращает код отклика и обновленный объект принтера `200 OK` в тексте [](../resources/printer.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="04d7b-193">If using delegated permissions, if successful, this method returns a `200 OK` response code and an updated [printer](../resources/printer.md) object in the response body.</span></span>

### <a name="application-permissions-and-ipp-payload"></a><span data-ttu-id="04d7b-194">Разрешения приложений и полезной нагрузки IPP</span><span class="sxs-lookup"><span data-stu-id="04d7b-194">Application permissions and IPP payload</span></span>

<span data-ttu-id="04d7b-195">При использовании разрешений приложений при успешном использовании этот метод возвращает `204 No content` код ответа.</span><span class="sxs-lookup"><span data-stu-id="04d7b-195">If using application permissions, if successful, this method returns `204 No content` response code.</span></span> <span data-ttu-id="04d7b-196">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="04d7b-196">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04d7b-197">Пример</span><span class="sxs-lookup"><span data-stu-id="04d7b-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="04d7b-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="04d7b-198">Request</span></span>
<span data-ttu-id="04d7b-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04d7b-199">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="04d7b-200">HTTP</span><span class="sxs-lookup"><span data-stu-id="04d7b-200">HTTP</span></span>](#tab/http)
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

---

### <a name="response"></a><span data-ttu-id="04d7b-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="04d7b-201">Response</span></span>
<span data-ttu-id="04d7b-202">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="04d7b-202">The following is an example of the response.</span></span>
><span data-ttu-id="04d7b-p112">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04d7b-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update printer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

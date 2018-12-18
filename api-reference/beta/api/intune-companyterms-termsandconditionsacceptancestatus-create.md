---
title: Создание объекта termsAndConditionsAcceptanceStatus
description: Создание объекта termsAndConditionsAcceptanceStatus.
author: tfitzmac
ms.openlocfilehash: 857e927d970f91070032dae95e699247aa7b11b3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340595"
---
# <a name="create-termsandconditionsacceptancestatus"></a><span data-ttu-id="d2ccf-103">Создание объекта termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="d2ccf-103">Create termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="d2ccf-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d2ccf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2ccf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2ccf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d2ccf-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d2ccf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2ccf-107">Создание объекта [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="d2ccf-107">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d2ccf-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d2ccf-108">Prerequisites</span></span>
<span data-ttu-id="d2ccf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2ccf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2ccf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2ccf-111">Permission type</span></span>|<span data-ttu-id="d2ccf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2ccf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2ccf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2ccf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d2ccf-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2ccf-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d2ccf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2ccf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2ccf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2ccf-116">Not supported.</span></span>|
|<span data-ttu-id="d2ccf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2ccf-117">Application</span></span>|<span data-ttu-id="d2ccf-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2ccf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2ccf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2ccf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="d2ccf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2ccf-120">Request headers</span></span>
|<span data-ttu-id="d2ccf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d2ccf-121">Header</span></span>|<span data-ttu-id="d2ccf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d2ccf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2ccf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2ccf-123">Authorization</span></span>|<span data-ttu-id="d2ccf-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d2ccf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2ccf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d2ccf-125">Accept</span></span>|<span data-ttu-id="d2ccf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d2ccf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2ccf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2ccf-127">Request body</span></span>
<span data-ttu-id="d2ccf-128">В тексте запроса добавьте представление объекта termsAndConditionsAcceptanceStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2ccf-128">In the request body, supply a JSON representation for the termsAndConditionsAcceptanceStatus object.</span></span>

<span data-ttu-id="d2ccf-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта termsAndConditionsAcceptanceStatus.</span><span class="sxs-lookup"><span data-stu-id="d2ccf-129">The following table shows the properties that are required when you create the termsAndConditionsAcceptanceStatus.</span></span>

|<span data-ttu-id="d2ccf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2ccf-130">Property</span></span>|<span data-ttu-id="d2ccf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d2ccf-131">Type</span></span>|<span data-ttu-id="d2ccf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d2ccf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2ccf-133">id</span><span class="sxs-lookup"><span data-stu-id="d2ccf-133">id</span></span>|<span data-ttu-id="d2ccf-134">String</span><span class="sxs-lookup"><span data-stu-id="d2ccf-134">String</span></span>|<span data-ttu-id="d2ccf-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="d2ccf-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="d2ccf-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="d2ccf-136">userDisplayName</span></span>|<span data-ttu-id="d2ccf-137">String</span><span class="sxs-lookup"><span data-stu-id="d2ccf-137">String</span></span>|<span data-ttu-id="d2ccf-138">Отображает имя пользователя, чье принятие представлено объектом.</span><span class="sxs-lookup"><span data-stu-id="d2ccf-138">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="d2ccf-139">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="d2ccf-139">acceptedVersion</span></span>|<span data-ttu-id="d2ccf-140">Int32</span><span class="sxs-lookup"><span data-stu-id="d2ccf-140">Int32</span></span>|<span data-ttu-id="d2ccf-141">Номер последней версии условий, принятых пользователем.</span><span class="sxs-lookup"><span data-stu-id="d2ccf-141">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="d2ccf-142">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="d2ccf-142">acceptedDateTime</span></span>|<span data-ttu-id="d2ccf-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2ccf-143">DateTimeOffset</span></span>|<span data-ttu-id="d2ccf-144">Дата и время последнего принятия условий пользователем.</span><span class="sxs-lookup"><span data-stu-id="d2ccf-144">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="d2ccf-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2ccf-145">Response</span></span>
<span data-ttu-id="d2ccf-146">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d2ccf-146">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2ccf-147">Пример</span><span class="sxs-lookup"><span data-stu-id="d2ccf-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="d2ccf-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2ccf-148">Request</span></span>
<span data-ttu-id="d2ccf-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2ccf-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="d2ccf-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="d2ccf-150">Response</span></span>
<span data-ttu-id="d2ccf-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d2ccf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```






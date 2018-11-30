---
title: Обновление объекта reportRoot
description: Обновление свойств объекта reportRoot.
ms.openlocfilehash: 199ebfa724b5cdfc510aa0d82f8ae3bfd87aee58
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078008"
---
# <a name="update-reportroot"></a><span data-ttu-id="801ac-103">Обновление объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="801ac-103">Update reportRoot</span></span>

> <span data-ttu-id="801ac-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="801ac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="801ac-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="801ac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="801ac-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="801ac-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="801ac-107">Обновление свойств объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="801ac-107">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="801ac-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="801ac-108">Prerequisites</span></span>
<span data-ttu-id="801ac-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="801ac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="801ac-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="801ac-111">Permission type</span></span>|<span data-ttu-id="801ac-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="801ac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="801ac-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="801ac-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="801ac-114">&nbsp;&nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="801ac-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="801ac-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="801ac-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="801ac-116">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="801ac-116">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="801ac-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="801ac-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="801ac-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="801ac-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="801ac-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="801ac-119">Not supported.</span></span>|
|<span data-ttu-id="801ac-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="801ac-120">Application</span></span>|<span data-ttu-id="801ac-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="801ac-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="801ac-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="801ac-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="801ac-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="801ac-123">Request headers</span></span>
|<span data-ttu-id="801ac-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="801ac-124">Header</span></span>|<span data-ttu-id="801ac-125">Значение</span><span class="sxs-lookup"><span data-stu-id="801ac-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="801ac-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="801ac-126">Authorization</span></span>|<span data-ttu-id="801ac-127">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="801ac-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="801ac-128">Accept</span><span class="sxs-lookup"><span data-stu-id="801ac-128">Accept</span></span>|<span data-ttu-id="801ac-129">application/json</span><span class="sxs-lookup"><span data-stu-id="801ac-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="801ac-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="801ac-130">Request body</span></span>
<span data-ttu-id="801ac-131">В тексте запроса добавьте представление объекта [reportRoot](../resources/intune-shared-reportroot.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="801ac-131">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

<span data-ttu-id="801ac-132">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="801ac-132">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-shared-reportroot.md).</span></span>

|<span data-ttu-id="801ac-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="801ac-133">Property</span></span>|<span data-ttu-id="801ac-134">Тип</span><span class="sxs-lookup"><span data-stu-id="801ac-134">Type</span></span>|<span data-ttu-id="801ac-135">Описание</span><span class="sxs-lookup"><span data-stu-id="801ac-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="801ac-136">id</span><span class="sxs-lookup"><span data-stu-id="801ac-136">id</span></span>|<span data-ttu-id="801ac-137">String</span><span class="sxs-lookup"><span data-stu-id="801ac-137">String</span></span>|<span data-ttu-id="801ac-138">Уникальный идентификатор для этого объекта.</span><span class="sxs-lookup"><span data-stu-id="801ac-138">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="801ac-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="801ac-139">Response</span></span>
<span data-ttu-id="801ac-140">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [reportRoot](../resources/intune-shared-reportroot.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="801ac-140">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="801ac-141">Пример</span><span class="sxs-lookup"><span data-stu-id="801ac-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="801ac-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="801ac-142">Request</span></span>
<span data-ttu-id="801ac-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="801ac-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="801ac-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="801ac-144">Response</span></span>
<span data-ttu-id="801ac-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="801ac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```




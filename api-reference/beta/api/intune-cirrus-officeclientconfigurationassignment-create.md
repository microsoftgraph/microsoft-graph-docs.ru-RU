---
title: Создание officeClientConfigurationAssignment
description: Добавьте целевой группе существующую политику.
ms.openlocfilehash: 60416fe200214864c063a9fae739d5f7bd436a69
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077863"
---
# <a name="create-officeclientconfigurationassignment"></a><span data-ttu-id="47bed-103">Создание officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="47bed-103">Create officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="47bed-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="47bed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47bed-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47bed-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="47bed-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="47bed-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47bed-107">Добавьте целевой группе существующую политику.</span><span class="sxs-lookup"><span data-stu-id="47bed-107">Add a target group to an existing policy.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="47bed-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="47bed-108">Prerequisites</span></span>
<span data-ttu-id="47bed-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47bed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47bed-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47bed-111">Permission type</span></span>|<span data-ttu-id="47bed-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="47bed-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47bed-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47bed-113">Delegated (work or school account)</span></span>|<span data-ttu-id="47bed-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47bed-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="47bed-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47bed-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47bed-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47bed-116">Not supported.</span></span>|
|<span data-ttu-id="47bed-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47bed-117">Application</span></span>|<span data-ttu-id="47bed-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47bed-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47bed-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47bed-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{key}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="47bed-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47bed-120">Request headers</span></span>
|<span data-ttu-id="47bed-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47bed-121">Header</span></span>|<span data-ttu-id="47bed-122">Значение</span><span class="sxs-lookup"><span data-stu-id="47bed-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47bed-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="47bed-123">Authorization</span></span>|<span data-ttu-id="47bed-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="47bed-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47bed-125">Accept</span><span class="sxs-lookup"><span data-stu-id="47bed-125">Accept</span></span>|<span data-ttu-id="47bed-126">application/json</span><span class="sxs-lookup"><span data-stu-id="47bed-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47bed-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47bed-127">Request body</span></span>
<span data-ttu-id="47bed-128">В тексте запроса укажите представление JSON для объекта officeClientConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="47bed-128">In the request body, supply a JSON representation for the officeClientConfigurationAssignment object.</span></span>

<span data-ttu-id="47bed-129">В следующей таблице показаны свойства, которые необходимы для создания officeClientConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="47bed-129">The following table shows the properties that are required when you create the officeClientConfigurationAssignment.</span></span>

|<span data-ttu-id="47bed-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="47bed-130">Property</span></span>|<span data-ttu-id="47bed-131">Тип</span><span class="sxs-lookup"><span data-stu-id="47bed-131">Type</span></span>|<span data-ttu-id="47bed-132">Описание</span><span class="sxs-lookup"><span data-stu-id="47bed-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47bed-133">id</span><span class="sxs-lookup"><span data-stu-id="47bed-133">id</span></span>|<span data-ttu-id="47bed-134">String</span><span class="sxs-lookup"><span data-stu-id="47bed-134">String</span></span>|<span data-ttu-id="47bed-135">Идентификатор OfficeConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="47bed-135">Id of the OfficeConfigurationAssignment.</span></span>|
|<span data-ttu-id="47bed-136">target</span><span class="sxs-lookup"><span data-stu-id="47bed-136">target</span></span>|[<span data-ttu-id="47bed-137">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="47bed-137">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="47bed-138">Назначение целевой, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="47bed-138">The target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="47bed-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="47bed-139">Response</span></span>
<span data-ttu-id="47bed-140">Успешно завершена, этот метод возвращает `200 Created` код ответа и объект [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="47bed-140">If successful, this method returns a `200 Created` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47bed-141">Пример</span><span class="sxs-lookup"><span data-stu-id="47bed-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="47bed-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="47bed-142">Request</span></span>
<span data-ttu-id="47bed-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47bed-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="47bed-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="47bed-144">Response</span></span>
<span data-ttu-id="47bed-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="47bed-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "id": "804730f3-30f3-8047-f330-4780f3304780",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```




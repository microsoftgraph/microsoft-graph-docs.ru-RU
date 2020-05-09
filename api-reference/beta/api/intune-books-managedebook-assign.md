---
title: Действие assign
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 675b146e14516d897672e27cd38ea111cc150b49
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44175107"
---
# <a name="assign-action"></a><span data-ttu-id="4e372-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="4e372-103">assign action</span></span>

<span data-ttu-id="4e372-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e372-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e372-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e372-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e372-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4e372-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e372-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4e372-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e372-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4e372-108">Prerequisites</span></span>
<span data-ttu-id="4e372-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e372-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e372-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e372-111">Permission type</span></span>|<span data-ttu-id="4e372-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e372-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e372-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e372-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e372-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e372-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4e372-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e372-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e372-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e372-116">Not supported.</span></span>|
|<span data-ttu-id="4e372-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e372-117">Application</span></span>|<span data-ttu-id="4e372-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e372-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e372-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e372-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="4e372-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4e372-120">Request headers</span></span>
|<span data-ttu-id="4e372-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4e372-121">Header</span></span>|<span data-ttu-id="4e372-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4e372-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e372-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e372-123">Authorization</span></span>|<span data-ttu-id="4e372-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e372-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e372-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4e372-125">Accept</span></span>|<span data-ttu-id="4e372-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4e372-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e372-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4e372-127">Request body</span></span>
<span data-ttu-id="4e372-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e372-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4e372-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="4e372-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4e372-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e372-130">Property</span></span>|<span data-ttu-id="4e372-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4e372-131">Type</span></span>|<span data-ttu-id="4e372-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4e372-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e372-133">managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="4e372-133">managedEBookAssignments</span></span>|<span data-ttu-id="4e372-134">Коллекция [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4e372-134">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="4e372-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4e372-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4e372-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="4e372-136">Response</span></span>
<span data-ttu-id="4e372-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4e372-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4e372-138">Пример</span><span class="sxs-lookup"><span data-stu-id="4e372-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e372-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e372-139">Request</span></span>
<span data-ttu-id="4e372-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e372-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assign

Content-type: application/json
Content-length: 312

{
  "managedEBookAssignments": [
    {
      "@odata.type": "#microsoft.graph.managedEBookAssignment",
      "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
      },
      "installIntent": "required"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="4e372-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e372-141">Response</span></span>
<span data-ttu-id="4e372-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4e372-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




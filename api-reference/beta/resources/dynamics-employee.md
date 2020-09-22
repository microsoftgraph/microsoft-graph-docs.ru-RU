---
title: Тип ресурса Employees
description: Объект Employee в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: d404a1ede257f3a31371dba31c37ff329452fccd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071341"
---
# <a name="employees-resource-type"></a><span data-ttu-id="e36a1-103">Тип ресурса Employees</span><span class="sxs-lookup"><span data-stu-id="e36a1-103">employees resource type</span></span>

<span data-ttu-id="e36a1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e36a1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e36a1-105">Представляет сотрудника в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="e36a1-105">Represents an employee in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="e36a1-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e36a1-106">Methods</span></span>

| <span data-ttu-id="e36a1-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e36a1-107">Method</span></span>                                              | <span data-ttu-id="e36a1-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e36a1-108">Return Type</span></span>|<span data-ttu-id="e36a1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e36a1-109">Description</span></span>               |
|:----------------------------------------------------|:-----------|:-------------------------|
|[<span data-ttu-id="e36a1-110">Получение сотрудников</span><span class="sxs-lookup"><span data-stu-id="e36a1-110">Get employees</span></span>](../api/dynamics-employee-get.md)      |<span data-ttu-id="e36a1-111">сотрудников</span><span class="sxs-lookup"><span data-stu-id="e36a1-111">employees</span></span>  |<span data-ttu-id="e36a1-112">Получение объекта Employee.</span><span class="sxs-lookup"><span data-stu-id="e36a1-112">Get an employee object.</span></span>   |
|[<span data-ttu-id="e36a1-113">Учет сотрудников</span><span class="sxs-lookup"><span data-stu-id="e36a1-113">Post employees</span></span>](../api/dynamics-create-employee.md)  |<span data-ttu-id="e36a1-114">сотрудников</span><span class="sxs-lookup"><span data-stu-id="e36a1-114">employees</span></span>  |<span data-ttu-id="e36a1-115">Создание объекта Employee.</span><span class="sxs-lookup"><span data-stu-id="e36a1-115">Create an employee object.</span></span>|
|[<span data-ttu-id="e36a1-116">Обновление сотрудников</span><span class="sxs-lookup"><span data-stu-id="e36a1-116">Patch employees</span></span>](../api/dynamics-employee-update.md) |<span data-ttu-id="e36a1-117">сотрудников</span><span class="sxs-lookup"><span data-stu-id="e36a1-117">employees</span></span>  |<span data-ttu-id="e36a1-118">Обновление объекта Employee.</span><span class="sxs-lookup"><span data-stu-id="e36a1-118">Update an employee object.</span></span>|
|[<span data-ttu-id="e36a1-119">Удаление сотрудников</span><span class="sxs-lookup"><span data-stu-id="e36a1-119">Delete employees</span></span>](../api/dynamics-employee-delete.md)|<span data-ttu-id="e36a1-120">Нет</span><span class="sxs-lookup"><span data-stu-id="e36a1-120">none</span></span>       |<span data-ttu-id="e36a1-121">Удаление объекта Employee.</span><span class="sxs-lookup"><span data-stu-id="e36a1-121">Delete an employee object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e36a1-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="e36a1-122">Properties</span></span>
| <span data-ttu-id="e36a1-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="e36a1-123">Property</span></span>           | <span data-ttu-id="e36a1-124">Тип</span><span class="sxs-lookup"><span data-stu-id="e36a1-124">Type</span></span>   |<span data-ttu-id="e36a1-125">Описание</span><span class="sxs-lookup"><span data-stu-id="e36a1-125">Description</span></span>                                            |
|:-------------------|:-------|:------------------------------------------------------|
|<span data-ttu-id="e36a1-126">id</span><span class="sxs-lookup"><span data-stu-id="e36a1-126">id</span></span>                  |<span data-ttu-id="e36a1-127">GUID</span><span class="sxs-lookup"><span data-stu-id="e36a1-127">GUID</span></span>    |<span data-ttu-id="e36a1-128">Идентификатор сотрудника.</span><span class="sxs-lookup"><span data-stu-id="e36a1-128">The employee ID.</span></span> <span data-ttu-id="e36a1-129">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="e36a1-129">Non-editable.</span></span>                         |
|<span data-ttu-id="e36a1-130">число</span><span class="sxs-lookup"><span data-stu-id="e36a1-130">number</span></span>              |<span data-ttu-id="e36a1-131">string</span><span class="sxs-lookup"><span data-stu-id="e36a1-131">string</span></span>  |<span data-ttu-id="e36a1-132">Номер сотрудника.</span><span class="sxs-lookup"><span data-stu-id="e36a1-132">The employee number.</span></span> <span data-ttu-id="e36a1-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e36a1-133">Read-Only.</span></span>                        |
|<span data-ttu-id="e36a1-134">displayName</span><span class="sxs-lookup"><span data-stu-id="e36a1-134">displayName</span></span>         |<span data-ttu-id="e36a1-135">string</span><span class="sxs-lookup"><span data-stu-id="e36a1-135">string</span></span>  |<span data-ttu-id="e36a1-136">Сотрудник givenName + фамилия.</span><span class="sxs-lookup"><span data-stu-id="e36a1-136">The employee givenName + surname.</span></span> <span data-ttu-id="e36a1-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e36a1-137">Read-Only.</span></span>           |
|<span data-ttu-id="e36a1-138">givenName;</span><span class="sxs-lookup"><span data-stu-id="e36a1-138">givenName</span></span>           |<span data-ttu-id="e36a1-139">string</span><span class="sxs-lookup"><span data-stu-id="e36a1-139">string</span></span>  |<span data-ttu-id="e36a1-140">Заданное имя сотрудника.</span><span class="sxs-lookup"><span data-stu-id="e36a1-140">The given name of the employee.</span></span>                        |
|<span data-ttu-id="e36a1-141">middleName</span><span class="sxs-lookup"><span data-stu-id="e36a1-141">middleName</span></span>          |<span data-ttu-id="e36a1-142">string</span><span class="sxs-lookup"><span data-stu-id="e36a1-142">string</span></span>  |<span data-ttu-id="e36a1-143">Отчество сотрудника.</span><span class="sxs-lookup"><span data-stu-id="e36a1-143">The middle name of the employee.</span></span>                       |
|<span data-ttu-id="e36a1-144">surname</span><span class="sxs-lookup"><span data-stu-id="e36a1-144">surname</span></span>             |<span data-ttu-id="e36a1-145">string</span><span class="sxs-lookup"><span data-stu-id="e36a1-145">string</span></span>  |<span data-ttu-id="e36a1-146">Фамилия сотрудника</span><span class="sxs-lookup"><span data-stu-id="e36a1-146">The surname of the employee</span></span>                            |
|<span data-ttu-id="e36a1-147">jobTitle;</span><span class="sxs-lookup"><span data-stu-id="e36a1-147">jobTitle</span></span>            |<span data-ttu-id="e36a1-148">string</span><span class="sxs-lookup"><span data-stu-id="e36a1-148">string</span></span>  |<span data-ttu-id="e36a1-149">Полное имя сотрудника</span><span class="sxs-lookup"><span data-stu-id="e36a1-149">The full name of the employee</span></span>                          |
|<span data-ttu-id="e36a1-150">address</span><span class="sxs-lookup"><span data-stu-id="e36a1-150">address</span></span>             |[<span data-ttu-id="e36a1-151">Навигационная. посталаддресс</span><span class="sxs-lookup"><span data-stu-id="e36a1-151">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="e36a1-152">Указывает адрес сотрудника.</span><span class="sxs-lookup"><span data-stu-id="e36a1-152">Specifies the employee's address.</span></span> <span data-ttu-id="e36a1-153">Этот адрес будет отображаться во всех документах ресурсов для сотрудника.</span><span class="sxs-lookup"><span data-stu-id="e36a1-153">This address will appear on all resource documents for the employee.</span></span>|
|<span data-ttu-id="e36a1-154">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="e36a1-154">phoneNumber</span></span>         |<span data-ttu-id="e36a1-155">string</span><span class="sxs-lookup"><span data-stu-id="e36a1-155">string</span></span>  |<span data-ttu-id="e36a1-156">Указывает номер телефона сотрудника.</span><span class="sxs-lookup"><span data-stu-id="e36a1-156">Specifies the employee's telephone number.</span></span>             |
|<span data-ttu-id="e36a1-157">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="e36a1-157">mobilePhone</span></span>         |<span data-ttu-id="e36a1-158">string</span><span class="sxs-lookup"><span data-stu-id="e36a1-158">string</span></span>  |<span data-ttu-id="e36a1-159">Указывает номер мобильного телефона сотрудника.</span><span class="sxs-lookup"><span data-stu-id="e36a1-159">Specifies the employee's mobile telephone number.</span></span>      |
|<span data-ttu-id="e36a1-160">email</span><span class="sxs-lookup"><span data-stu-id="e36a1-160">email</span></span>               |<span data-ttu-id="e36a1-161">строка</span><span class="sxs-lookup"><span data-stu-id="e36a1-161">string</span></span>  |<span data-ttu-id="e36a1-162">Указывает адрес электронной почты сотрудника.</span><span class="sxs-lookup"><span data-stu-id="e36a1-162">Specifies the employee's email address.</span></span>                |
|<span data-ttu-id="e36a1-163">персоналемаил</span><span class="sxs-lookup"><span data-stu-id="e36a1-163">personalEmail</span></span>       |<span data-ttu-id="e36a1-164">string</span><span class="sxs-lookup"><span data-stu-id="e36a1-164">string</span></span>  |<span data-ttu-id="e36a1-165">Указывает личный адрес электронной почты сотрудника.</span><span class="sxs-lookup"><span data-stu-id="e36a1-165">Specifies the employee's personal email address.</span></span>       |
|<span data-ttu-id="e36a1-166">емплойментдате</span><span class="sxs-lookup"><span data-stu-id="e36a1-166">employmentDate</span></span>      |<span data-ttu-id="e36a1-167">date</span><span class="sxs-lookup"><span data-stu-id="e36a1-167">date</span></span>    |<span data-ttu-id="e36a1-168">Указывает дату начала работы сотрудника в компании.</span><span class="sxs-lookup"><span data-stu-id="e36a1-168">Specifies the date when the employee began to work for the company.</span></span>|
|<span data-ttu-id="e36a1-169">терминатиондате</span><span class="sxs-lookup"><span data-stu-id="e36a1-169">terminationDate</span></span>     |<span data-ttu-id="e36a1-170">date</span><span class="sxs-lookup"><span data-stu-id="e36a1-170">date</span></span>    |<span data-ttu-id="e36a1-171">Указывает дату увольнения сотрудника, например из-за увольнения или увольнения.</span><span class="sxs-lookup"><span data-stu-id="e36a1-171">Specifies the date when the employee was terminated, due to retirement or dismissal, for example.</span></span>|
|<span data-ttu-id="e36a1-172">status</span><span class="sxs-lookup"><span data-stu-id="e36a1-172">status</span></span>              |<span data-ttu-id="e36a1-173">string</span><span class="sxs-lookup"><span data-stu-id="e36a1-173">string</span></span>  |<span data-ttu-id="e36a1-174">Указывает состояние сотрудника.</span><span class="sxs-lookup"><span data-stu-id="e36a1-174">Specifies the employee's status.</span></span> <span data-ttu-id="e36a1-175">Возможные значения: активные, неактивные или прерванные</span><span class="sxs-lookup"><span data-stu-id="e36a1-175">Possible values are Active, Inactive or Terminated</span></span>|
|<span data-ttu-id="e36a1-176">birthDate</span><span class="sxs-lookup"><span data-stu-id="e36a1-176">birthDate</span></span>           |<span data-ttu-id="e36a1-177">date</span><span class="sxs-lookup"><span data-stu-id="e36a1-177">date</span></span>    |<span data-ttu-id="e36a1-178">Указывает дату рождения сотрудника.</span><span class="sxs-lookup"><span data-stu-id="e36a1-178">Specifies the employee's date of birth.</span></span>                |
|<span data-ttu-id="e36a1-179">графические</span><span class="sxs-lookup"><span data-stu-id="e36a1-179">picture</span></span>             |<span data-ttu-id="e36a1-180">stream</span><span class="sxs-lookup"><span data-stu-id="e36a1-180">stream</span></span>  |<span data-ttu-id="e36a1-181">Фотография сотрудника.</span><span class="sxs-lookup"><span data-stu-id="e36a1-181">The employee picture.</span></span> <span data-ttu-id="e36a1-182">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e36a1-182">Read-Only.</span></span>                       |
|<span data-ttu-id="e36a1-183">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e36a1-183">lastModifiedDateTime</span></span>|<span data-ttu-id="e36a1-184">datetime</span><span class="sxs-lookup"><span data-stu-id="e36a1-184">datetime</span></span>|<span data-ttu-id="e36a1-185">Дата и время последнего изменения сотрудника.</span><span class="sxs-lookup"><span data-stu-id="e36a1-185">The last datetime the employee was modified.</span></span> <span data-ttu-id="e36a1-186">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e36a1-186">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="e36a1-187">Отношения</span><span class="sxs-lookup"><span data-stu-id="e36a1-187">Relationships</span></span>
<span data-ttu-id="e36a1-188">Нет</span><span class="sxs-lookup"><span data-stu-id="e36a1-188">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e36a1-189">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e36a1-189">JSON representation</span></span>

<span data-ttu-id="e36a1-190">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e36a1-190">Here is a JSON representation of the resource.</span></span>


```json
{
    "id": "GUID",
    "number": "string",
    "displayName": "string",
    "givenName": "string",
    "middleName": "string",
    "surname": "string",
    "jobTitle": "string",
    "address": "NAV.PostalAddress",
    "phoneNumber": "string",
    "mobilePhone": "string",
    "email": "string",
    "personalEmail": "string",
    "employmentDate": "date",
    "terminationDate": "date",
    "status": "string",
    "birthDate": "date",
    "picture": "stream",
    "lastModifiedDateTime": "datetime"
}

```




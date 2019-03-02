---
title: Тип ресурса Employees
description: Объект Employee в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 865da0c1e1256e2ba2a25902e37a00da9081eedf
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366657"
---
# <a name="employees-resource-type"></a><span data-ttu-id="c1c8b-103">Тип ресурса Employees</span><span class="sxs-lookup"><span data-stu-id="c1c8b-103">employees resource type</span></span>
<span data-ttu-id="c1c8b-104">Представляет сотрудника в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="c1c8b-104">Represents an employee in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="c1c8b-105">Методы</span><span class="sxs-lookup"><span data-stu-id="c1c8b-105">Methods</span></span>

| <span data-ttu-id="c1c8b-106">Метод</span><span class="sxs-lookup"><span data-stu-id="c1c8b-106">Method</span></span>                                              | <span data-ttu-id="c1c8b-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c1c8b-107">Return Type</span></span>|<span data-ttu-id="c1c8b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c1c8b-108">Description</span></span>               |
|:----------------------------------------------------|:-----------|:-------------------------|
|[<span data-ttu-id="c1c8b-109">Получение сотрудников</span><span class="sxs-lookup"><span data-stu-id="c1c8b-109">Get employees</span></span>](../api/dynamics-employee-get.md)      |<span data-ttu-id="c1c8b-110">сотрудников</span><span class="sxs-lookup"><span data-stu-id="c1c8b-110">employees</span></span>  |<span data-ttu-id="c1c8b-111">Получение объекта Employee.</span><span class="sxs-lookup"><span data-stu-id="c1c8b-111">Get an employee object.</span></span>   |
|[<span data-ttu-id="c1c8b-112">Учет сотрудников</span><span class="sxs-lookup"><span data-stu-id="c1c8b-112">Post employees</span></span>](../api/dynamics-create-employee.md)  |<span data-ttu-id="c1c8b-113">сотрудников</span><span class="sxs-lookup"><span data-stu-id="c1c8b-113">employees</span></span>  |<span data-ttu-id="c1c8b-114">Создание объекта Employee.</span><span class="sxs-lookup"><span data-stu-id="c1c8b-114">Create an employee object.</span></span>|
|[<span data-ttu-id="c1c8b-115">Обновление сотрудников</span><span class="sxs-lookup"><span data-stu-id="c1c8b-115">Patch employees</span></span>](../api/dynamics-employee-update.md) |<span data-ttu-id="c1c8b-116">сотрудников</span><span class="sxs-lookup"><span data-stu-id="c1c8b-116">employees</span></span>  |<span data-ttu-id="c1c8b-117">Обновление объекта Employee.</span><span class="sxs-lookup"><span data-stu-id="c1c8b-117">Update an employee object.</span></span>|
|[<span data-ttu-id="c1c8b-118">Удаление сотрудников</span><span class="sxs-lookup"><span data-stu-id="c1c8b-118">Delete employees</span></span>](../api/dynamics-employee-delete.md)|<span data-ttu-id="c1c8b-119">Нет</span><span class="sxs-lookup"><span data-stu-id="c1c8b-119">none</span></span>       |<span data-ttu-id="c1c8b-120">Удаление объекта Employee.</span><span class="sxs-lookup"><span data-stu-id="c1c8b-120">Delete an employee object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c1c8b-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="c1c8b-121">Properties</span></span>
| <span data-ttu-id="c1c8b-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1c8b-122">Property</span></span>           | <span data-ttu-id="c1c8b-123">Тип</span><span class="sxs-lookup"><span data-stu-id="c1c8b-123">Type</span></span>   |<span data-ttu-id="c1c8b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c1c8b-124">Description</span></span>                                            |
|:-------------------|:-------|:------------------------------------------------------|
|<span data-ttu-id="c1c8b-125">id</span><span class="sxs-lookup"><span data-stu-id="c1c8b-125">id</span></span>                  |<span data-ttu-id="c1c8b-126">GUID</span><span class="sxs-lookup"><span data-stu-id="c1c8b-126">GUID</span></span>    |<span data-ttu-id="c1c8b-127">Идентификатор сотрудника.</span><span class="sxs-lookup"><span data-stu-id="c1c8b-127">The employee ID.</span></span> <span data-ttu-id="c1c8b-128">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="c1c8b-128">Non-editable.</span></span>                         |
|<span data-ttu-id="c1c8b-129">number</span><span class="sxs-lookup"><span data-stu-id="c1c8b-129">number</span></span>              |<span data-ttu-id="c1c8b-130">строка</span><span class="sxs-lookup"><span data-stu-id="c1c8b-130">string</span></span>  |<span data-ttu-id="c1c8b-131">Номер сотрудника.</span><span class="sxs-lookup"><span data-stu-id="c1c8b-131">The employee number.</span></span> <span data-ttu-id="c1c8b-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c1c8b-132">Read-Only.</span></span>                        |
|<span data-ttu-id="c1c8b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c1c8b-133">displayName</span></span>         |<span data-ttu-id="c1c8b-134">строка</span><span class="sxs-lookup"><span data-stu-id="c1c8b-134">string</span></span>  |<span data-ttu-id="c1c8b-135">Сотрудник givenName + фамилия.</span><span class="sxs-lookup"><span data-stu-id="c1c8b-135">The employee givenName + surname.</span></span> <span data-ttu-id="c1c8b-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c1c8b-136">Read-Only.</span></span>           |
|<span data-ttu-id="c1c8b-137">givenName;</span><span class="sxs-lookup"><span data-stu-id="c1c8b-137">givenName</span></span>           |<span data-ttu-id="c1c8b-138">строка</span><span class="sxs-lookup"><span data-stu-id="c1c8b-138">string</span></span>  |<span data-ttu-id="c1c8b-139">Заданное имя сотрудника.</span><span class="sxs-lookup"><span data-stu-id="c1c8b-139">The given name of the employee.</span></span>                        |
|<span data-ttu-id="c1c8b-140">middleName</span><span class="sxs-lookup"><span data-stu-id="c1c8b-140">middleName</span></span>          |<span data-ttu-id="c1c8b-141">строка</span><span class="sxs-lookup"><span data-stu-id="c1c8b-141">string</span></span>  |<span data-ttu-id="c1c8b-142">Отчество сотрудника.</span><span class="sxs-lookup"><span data-stu-id="c1c8b-142">The middle name of the employee.</span></span>                       |
|<span data-ttu-id="c1c8b-143">surname</span><span class="sxs-lookup"><span data-stu-id="c1c8b-143">surname</span></span>             |<span data-ttu-id="c1c8b-144">строка</span><span class="sxs-lookup"><span data-stu-id="c1c8b-144">string</span></span>  |<span data-ttu-id="c1c8b-145">Фамилия сотрудника</span><span class="sxs-lookup"><span data-stu-id="c1c8b-145">The surname of the employee</span></span>                            |
|<span data-ttu-id="c1c8b-146">jobTitle;</span><span class="sxs-lookup"><span data-stu-id="c1c8b-146">jobTitle</span></span>            |<span data-ttu-id="c1c8b-147">строка</span><span class="sxs-lookup"><span data-stu-id="c1c8b-147">string</span></span>  |<span data-ttu-id="c1c8b-148">Полное имя сотрудника</span><span class="sxs-lookup"><span data-stu-id="c1c8b-148">The full name of the employee</span></span>                          |
|<span data-ttu-id="c1c8b-149">address</span><span class="sxs-lookup"><span data-stu-id="c1c8b-149">address</span></span>             |[<span data-ttu-id="c1c8b-150">Навигационная. Посталаддресс</span><span class="sxs-lookup"><span data-stu-id="c1c8b-150">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="c1c8b-151">Указывает адрес сотрудника.</span><span class="sxs-lookup"><span data-stu-id="c1c8b-151">Specifies the employee's address.</span></span> <span data-ttu-id="c1c8b-152">Этот адрес будет отображаться во всех документах ресурсов для сотрудника.</span><span class="sxs-lookup"><span data-stu-id="c1c8b-152">This address will appear on all resource documents for the employee.</span></span>|
|<span data-ttu-id="c1c8b-153">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="c1c8b-153">phoneNumber</span></span>         |<span data-ttu-id="c1c8b-154">строка</span><span class="sxs-lookup"><span data-stu-id="c1c8b-154">string</span></span>  |<span data-ttu-id="c1c8b-155">Указывает номер телефона сотрудника.</span><span class="sxs-lookup"><span data-stu-id="c1c8b-155">Specifies the employee's telephone number.</span></span>             |
|<span data-ttu-id="c1c8b-156">mobilePhone;</span><span class="sxs-lookup"><span data-stu-id="c1c8b-156">mobilePhone</span></span>         |<span data-ttu-id="c1c8b-157">строка</span><span class="sxs-lookup"><span data-stu-id="c1c8b-157">string</span></span>  |<span data-ttu-id="c1c8b-158">Указывает номер мобильного телефона сотрудника.</span><span class="sxs-lookup"><span data-stu-id="c1c8b-158">Specifies the employee's mobile telephone number.</span></span>      |
|<span data-ttu-id="c1c8b-159">email</span><span class="sxs-lookup"><span data-stu-id="c1c8b-159">email</span></span>               |<span data-ttu-id="c1c8b-160">строка</span><span class="sxs-lookup"><span data-stu-id="c1c8b-160">string</span></span>  |<span data-ttu-id="c1c8b-161">Указывает адрес электронной почты сотрудника.</span><span class="sxs-lookup"><span data-stu-id="c1c8b-161">Specifies the employee's email address.</span></span>                |
|<span data-ttu-id="c1c8b-162">Персоналемаил</span><span class="sxs-lookup"><span data-stu-id="c1c8b-162">personalEmail</span></span>       |<span data-ttu-id="c1c8b-163">строка</span><span class="sxs-lookup"><span data-stu-id="c1c8b-163">string</span></span>  |<span data-ttu-id="c1c8b-164">Указывает личный адрес электронной почты сотрудника.</span><span class="sxs-lookup"><span data-stu-id="c1c8b-164">Specifies the employee's personal email address.</span></span>       |
|<span data-ttu-id="c1c8b-165">Емплойментдате</span><span class="sxs-lookup"><span data-stu-id="c1c8b-165">employmentDate</span></span>      |<span data-ttu-id="c1c8b-166">дата</span><span class="sxs-lookup"><span data-stu-id="c1c8b-166">date</span></span>    |<span data-ttu-id="c1c8b-167">Указывает дату начала работы сотрудника в компании.</span><span class="sxs-lookup"><span data-stu-id="c1c8b-167">Specifies the date when the employee began to work for the company.</span></span>|
|<span data-ttu-id="c1c8b-168">Терминатиондате</span><span class="sxs-lookup"><span data-stu-id="c1c8b-168">terminationDate</span></span>     |<span data-ttu-id="c1c8b-169">дата</span><span class="sxs-lookup"><span data-stu-id="c1c8b-169">date</span></span>    |<span data-ttu-id="c1c8b-170">Указывает дату увольнения сотрудника, например из-за увольнения или увольнения.</span><span class="sxs-lookup"><span data-stu-id="c1c8b-170">Specifies the date when the employee was terminated, due to retirement or dismissal, for example.</span></span>|
|<span data-ttu-id="c1c8b-171">status</span><span class="sxs-lookup"><span data-stu-id="c1c8b-171">status</span></span>              |<span data-ttu-id="c1c8b-172">string</span><span class="sxs-lookup"><span data-stu-id="c1c8b-172">string</span></span>  |<span data-ttu-id="c1c8b-173">Указывает состояние сотрудника.</span><span class="sxs-lookup"><span data-stu-id="c1c8b-173">Specifies the employee's status.</span></span> <span data-ttu-id="c1c8b-174">Возможные значения: активные, неАктивные или прерванные</span><span class="sxs-lookup"><span data-stu-id="c1c8b-174">Possible values are Active, Inactive or Terminated</span></span>|
|<span data-ttu-id="c1c8b-175">birthDate</span><span class="sxs-lookup"><span data-stu-id="c1c8b-175">birthDate</span></span>           |<span data-ttu-id="c1c8b-176">дата</span><span class="sxs-lookup"><span data-stu-id="c1c8b-176">date</span></span>    |<span data-ttu-id="c1c8b-177">Указывает дату рождения сотрудника.</span><span class="sxs-lookup"><span data-stu-id="c1c8b-177">Specifies the employee's date of birth.</span></span>                |
|<span data-ttu-id="c1c8b-178">графические</span><span class="sxs-lookup"><span data-stu-id="c1c8b-178">picture</span></span>             |<span data-ttu-id="c1c8b-179">stream</span><span class="sxs-lookup"><span data-stu-id="c1c8b-179">stream</span></span>  |<span data-ttu-id="c1c8b-180">Фотография сотрудника.</span><span class="sxs-lookup"><span data-stu-id="c1c8b-180">The employee picture.</span></span> <span data-ttu-id="c1c8b-181">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c1c8b-181">Read-Only.</span></span>                       |
|<span data-ttu-id="c1c8b-182">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1c8b-182">lastModifiedDateTime</span></span>|<span data-ttu-id="c1c8b-183">отличным</span><span class="sxs-lookup"><span data-stu-id="c1c8b-183">datetime</span></span>|<span data-ttu-id="c1c8b-184">Дата и время последнего изменения сотрудника.</span><span class="sxs-lookup"><span data-stu-id="c1c8b-184">The last datetime the employee was modified.</span></span> <span data-ttu-id="c1c8b-185">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c1c8b-185">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="c1c8b-186">Отношения</span><span class="sxs-lookup"><span data-stu-id="c1c8b-186">Relationships</span></span>
<span data-ttu-id="c1c8b-187">Нет</span><span class="sxs-lookup"><span data-stu-id="c1c8b-187">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1c8b-188">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c1c8b-188">JSON representation</span></span>

<span data-ttu-id="c1c8b-189">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1c8b-189">Here is a JSON representation of the resource.</span></span>


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


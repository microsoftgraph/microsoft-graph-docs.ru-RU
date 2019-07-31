---
title: Тип ресурса Employees
description: Объект Employee в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 96d44856ad52c983e61181fc64b93477fbe79e6c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972952"
---
# <a name="employees-resource-type"></a><span data-ttu-id="f49d8-103">Тип ресурса Employees</span><span class="sxs-lookup"><span data-stu-id="f49d8-103">employees resource type</span></span>
<span data-ttu-id="f49d8-104">Представляет сотрудника в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="f49d8-104">Represents an employee in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="f49d8-105">Методы</span><span class="sxs-lookup"><span data-stu-id="f49d8-105">Methods</span></span>

| <span data-ttu-id="f49d8-106">Метод</span><span class="sxs-lookup"><span data-stu-id="f49d8-106">Method</span></span>                                              | <span data-ttu-id="f49d8-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f49d8-107">Return Type</span></span>|<span data-ttu-id="f49d8-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f49d8-108">Description</span></span>               |
|:----------------------------------------------------|:-----------|:-------------------------|
|[<span data-ttu-id="f49d8-109">Получение сотрудников</span><span class="sxs-lookup"><span data-stu-id="f49d8-109">Get employees</span></span>](../api/dynamics-employee-get.md)      |<span data-ttu-id="f49d8-110">сотрудников</span><span class="sxs-lookup"><span data-stu-id="f49d8-110">employees</span></span>  |<span data-ttu-id="f49d8-111">Получение объекта Employee.</span><span class="sxs-lookup"><span data-stu-id="f49d8-111">Get an employee object.</span></span>   |
|[<span data-ttu-id="f49d8-112">Учет сотрудников</span><span class="sxs-lookup"><span data-stu-id="f49d8-112">Post employees</span></span>](../api/dynamics-create-employee.md)  |<span data-ttu-id="f49d8-113">сотрудников</span><span class="sxs-lookup"><span data-stu-id="f49d8-113">employees</span></span>  |<span data-ttu-id="f49d8-114">Создание объекта Employee.</span><span class="sxs-lookup"><span data-stu-id="f49d8-114">Create an employee object.</span></span>|
|[<span data-ttu-id="f49d8-115">Обновление сотрудников</span><span class="sxs-lookup"><span data-stu-id="f49d8-115">Patch employees</span></span>](../api/dynamics-employee-update.md) |<span data-ttu-id="f49d8-116">сотрудников</span><span class="sxs-lookup"><span data-stu-id="f49d8-116">employees</span></span>  |<span data-ttu-id="f49d8-117">Обновление объекта Employee.</span><span class="sxs-lookup"><span data-stu-id="f49d8-117">Update an employee object.</span></span>|
|[<span data-ttu-id="f49d8-118">Удаление сотрудников</span><span class="sxs-lookup"><span data-stu-id="f49d8-118">Delete employees</span></span>](../api/dynamics-employee-delete.md)|<span data-ttu-id="f49d8-119">none</span><span class="sxs-lookup"><span data-stu-id="f49d8-119">none</span></span>       |<span data-ttu-id="f49d8-120">Удаление объекта Employee.</span><span class="sxs-lookup"><span data-stu-id="f49d8-120">Delete an employee object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f49d8-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="f49d8-121">Properties</span></span>
| <span data-ttu-id="f49d8-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="f49d8-122">Property</span></span>           | <span data-ttu-id="f49d8-123">Тип</span><span class="sxs-lookup"><span data-stu-id="f49d8-123">Type</span></span>   |<span data-ttu-id="f49d8-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f49d8-124">Description</span></span>                                            |
|:-------------------|:-------|:------------------------------------------------------|
|<span data-ttu-id="f49d8-125">id</span><span class="sxs-lookup"><span data-stu-id="f49d8-125">id</span></span>                  |<span data-ttu-id="f49d8-126">GUID</span><span class="sxs-lookup"><span data-stu-id="f49d8-126">GUID</span></span>    |<span data-ttu-id="f49d8-127">Идентификатор сотрудника.</span><span class="sxs-lookup"><span data-stu-id="f49d8-127">The employee ID.</span></span> <span data-ttu-id="f49d8-128">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="f49d8-128">Non-editable.</span></span>                         |
|<span data-ttu-id="f49d8-129">число</span><span class="sxs-lookup"><span data-stu-id="f49d8-129">number</span></span>              |<span data-ttu-id="f49d8-130">string</span><span class="sxs-lookup"><span data-stu-id="f49d8-130">string</span></span>  |<span data-ttu-id="f49d8-131">Номер сотрудника.</span><span class="sxs-lookup"><span data-stu-id="f49d8-131">The employee number.</span></span> <span data-ttu-id="f49d8-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f49d8-132">Read-Only.</span></span>                        |
|<span data-ttu-id="f49d8-133">displayName</span><span class="sxs-lookup"><span data-stu-id="f49d8-133">displayName</span></span>         |<span data-ttu-id="f49d8-134">string</span><span class="sxs-lookup"><span data-stu-id="f49d8-134">string</span></span>  |<span data-ttu-id="f49d8-135">Сотрудник givenName + фамилия.</span><span class="sxs-lookup"><span data-stu-id="f49d8-135">The employee givenName + surname.</span></span> <span data-ttu-id="f49d8-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f49d8-136">Read-Only.</span></span>           |
|<span data-ttu-id="f49d8-137">givenName</span><span class="sxs-lookup"><span data-stu-id="f49d8-137">givenName</span></span>           |<span data-ttu-id="f49d8-138">string</span><span class="sxs-lookup"><span data-stu-id="f49d8-138">string</span></span>  |<span data-ttu-id="f49d8-139">Заданное имя сотрудника.</span><span class="sxs-lookup"><span data-stu-id="f49d8-139">The given name of the employee.</span></span>                        |
|<span data-ttu-id="f49d8-140">middleName</span><span class="sxs-lookup"><span data-stu-id="f49d8-140">middleName</span></span>          |<span data-ttu-id="f49d8-141">string</span><span class="sxs-lookup"><span data-stu-id="f49d8-141">string</span></span>  |<span data-ttu-id="f49d8-142">Отчество сотрудника.</span><span class="sxs-lookup"><span data-stu-id="f49d8-142">The middle name of the employee.</span></span>                       |
|<span data-ttu-id="f49d8-143">surname</span><span class="sxs-lookup"><span data-stu-id="f49d8-143">surname</span></span>             |<span data-ttu-id="f49d8-144">string</span><span class="sxs-lookup"><span data-stu-id="f49d8-144">string</span></span>  |<span data-ttu-id="f49d8-145">Фамилия сотрудника</span><span class="sxs-lookup"><span data-stu-id="f49d8-145">The surname of the employee</span></span>                            |
|<span data-ttu-id="f49d8-146">jobTitle</span><span class="sxs-lookup"><span data-stu-id="f49d8-146">jobTitle</span></span>            |<span data-ttu-id="f49d8-147">string</span><span class="sxs-lookup"><span data-stu-id="f49d8-147">string</span></span>  |<span data-ttu-id="f49d8-148">Полное имя сотрудника</span><span class="sxs-lookup"><span data-stu-id="f49d8-148">The full name of the employee</span></span>                          |
|<span data-ttu-id="f49d8-149">address</span><span class="sxs-lookup"><span data-stu-id="f49d8-149">address</span></span>             |[<span data-ttu-id="f49d8-150">Навигационная. Посталаддресс</span><span class="sxs-lookup"><span data-stu-id="f49d8-150">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="f49d8-151">Указывает адрес сотрудника.</span><span class="sxs-lookup"><span data-stu-id="f49d8-151">Specifies the employee's address.</span></span> <span data-ttu-id="f49d8-152">Этот адрес будет отображаться во всех документах ресурсов для сотрудника.</span><span class="sxs-lookup"><span data-stu-id="f49d8-152">This address will appear on all resource documents for the employee.</span></span>|
|<span data-ttu-id="f49d8-153">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="f49d8-153">phoneNumber</span></span>         |<span data-ttu-id="f49d8-154">string</span><span class="sxs-lookup"><span data-stu-id="f49d8-154">string</span></span>  |<span data-ttu-id="f49d8-155">Указывает номер телефона сотрудника.</span><span class="sxs-lookup"><span data-stu-id="f49d8-155">Specifies the employee's telephone number.</span></span>             |
|<span data-ttu-id="f49d8-156">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="f49d8-156">mobilePhone</span></span>         |<span data-ttu-id="f49d8-157">string</span><span class="sxs-lookup"><span data-stu-id="f49d8-157">string</span></span>  |<span data-ttu-id="f49d8-158">Указывает номер мобильного телефона сотрудника.</span><span class="sxs-lookup"><span data-stu-id="f49d8-158">Specifies the employee's mobile telephone number.</span></span>      |
|<span data-ttu-id="f49d8-159">email</span><span class="sxs-lookup"><span data-stu-id="f49d8-159">email</span></span>               |<span data-ttu-id="f49d8-160">string</span><span class="sxs-lookup"><span data-stu-id="f49d8-160">string</span></span>  |<span data-ttu-id="f49d8-161">Указывает адрес электронной почты сотрудника.</span><span class="sxs-lookup"><span data-stu-id="f49d8-161">Specifies the employee's email address.</span></span>                |
|<span data-ttu-id="f49d8-162">Персоналемаил</span><span class="sxs-lookup"><span data-stu-id="f49d8-162">personalEmail</span></span>       |<span data-ttu-id="f49d8-163">string</span><span class="sxs-lookup"><span data-stu-id="f49d8-163">string</span></span>  |<span data-ttu-id="f49d8-164">Указывает личный адрес электронной почты сотрудника.</span><span class="sxs-lookup"><span data-stu-id="f49d8-164">Specifies the employee's personal email address.</span></span>       |
|<span data-ttu-id="f49d8-165">Емплойментдате</span><span class="sxs-lookup"><span data-stu-id="f49d8-165">employmentDate</span></span>      |<span data-ttu-id="f49d8-166">date</span><span class="sxs-lookup"><span data-stu-id="f49d8-166">date</span></span>    |<span data-ttu-id="f49d8-167">Указывает дату начала работы сотрудника в компании.</span><span class="sxs-lookup"><span data-stu-id="f49d8-167">Specifies the date when the employee began to work for the company.</span></span>|
|<span data-ttu-id="f49d8-168">Терминатиондате</span><span class="sxs-lookup"><span data-stu-id="f49d8-168">terminationDate</span></span>     |<span data-ttu-id="f49d8-169">date</span><span class="sxs-lookup"><span data-stu-id="f49d8-169">date</span></span>    |<span data-ttu-id="f49d8-170">Указывает дату увольнения сотрудника, например из-за увольнения или увольнения.</span><span class="sxs-lookup"><span data-stu-id="f49d8-170">Specifies the date when the employee was terminated, due to retirement or dismissal, for example.</span></span>|
|<span data-ttu-id="f49d8-171">status</span><span class="sxs-lookup"><span data-stu-id="f49d8-171">status</span></span>              |<span data-ttu-id="f49d8-172">string</span><span class="sxs-lookup"><span data-stu-id="f49d8-172">string</span></span>  |<span data-ttu-id="f49d8-173">Указывает состояние сотрудника.</span><span class="sxs-lookup"><span data-stu-id="f49d8-173">Specifies the employee's status.</span></span> <span data-ttu-id="f49d8-174">Возможные значения: активные, неактивные или прерванные</span><span class="sxs-lookup"><span data-stu-id="f49d8-174">Possible values are Active, Inactive or Terminated</span></span>|
|<span data-ttu-id="f49d8-175">birthDate</span><span class="sxs-lookup"><span data-stu-id="f49d8-175">birthDate</span></span>           |<span data-ttu-id="f49d8-176">date</span><span class="sxs-lookup"><span data-stu-id="f49d8-176">date</span></span>    |<span data-ttu-id="f49d8-177">Указывает дату рождения сотрудника.</span><span class="sxs-lookup"><span data-stu-id="f49d8-177">Specifies the employee's date of birth.</span></span>                |
|<span data-ttu-id="f49d8-178">графические</span><span class="sxs-lookup"><span data-stu-id="f49d8-178">picture</span></span>             |<span data-ttu-id="f49d8-179">stream</span><span class="sxs-lookup"><span data-stu-id="f49d8-179">stream</span></span>  |<span data-ttu-id="f49d8-180">Фотография сотрудника.</span><span class="sxs-lookup"><span data-stu-id="f49d8-180">The employee picture.</span></span> <span data-ttu-id="f49d8-181">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f49d8-181">Read-Only.</span></span>                       |
|<span data-ttu-id="f49d8-182">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f49d8-182">lastModifiedDateTime</span></span>|<span data-ttu-id="f49d8-183">отличным</span><span class="sxs-lookup"><span data-stu-id="f49d8-183">datetime</span></span>|<span data-ttu-id="f49d8-184">Дата и время последнего изменения сотрудника.</span><span class="sxs-lookup"><span data-stu-id="f49d8-184">The last datetime the employee was modified.</span></span> <span data-ttu-id="f49d8-185">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f49d8-185">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="f49d8-186">Отношения</span><span class="sxs-lookup"><span data-stu-id="f49d8-186">Relationships</span></span>
<span data-ttu-id="f49d8-187">Нет</span><span class="sxs-lookup"><span data-stu-id="f49d8-187">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f49d8-188">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f49d8-188">JSON representation</span></span>

<span data-ttu-id="f49d8-189">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f49d8-189">Here is a JSON representation of the resource.</span></span>


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


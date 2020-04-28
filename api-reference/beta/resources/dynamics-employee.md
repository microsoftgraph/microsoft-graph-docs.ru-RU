---
title: Тип ресурса Employees
description: Объект Employee в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 84fccbcb9d60c97a2ce0079a9ba773a8400a8069
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42504085"
---
# <a name="employees-resource-type"></a><span data-ttu-id="ea049-103">Тип ресурса Employees</span><span class="sxs-lookup"><span data-stu-id="ea049-103">employees resource type</span></span>

<span data-ttu-id="ea049-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea049-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea049-105">Представляет сотрудника в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="ea049-105">Represents an employee in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="ea049-106">Методы</span><span class="sxs-lookup"><span data-stu-id="ea049-106">Methods</span></span>

| <span data-ttu-id="ea049-107">Метод</span><span class="sxs-lookup"><span data-stu-id="ea049-107">Method</span></span>                                              | <span data-ttu-id="ea049-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ea049-108">Return Type</span></span>|<span data-ttu-id="ea049-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ea049-109">Description</span></span>               |
|:----------------------------------------------------|:-----------|:-------------------------|
|[<span data-ttu-id="ea049-110">Получение сотрудников</span><span class="sxs-lookup"><span data-stu-id="ea049-110">Get employees</span></span>](../api/dynamics-employee-get.md)      |<span data-ttu-id="ea049-111">сотрудников</span><span class="sxs-lookup"><span data-stu-id="ea049-111">employees</span></span>  |<span data-ttu-id="ea049-112">Получение объекта Employee.</span><span class="sxs-lookup"><span data-stu-id="ea049-112">Get an employee object.</span></span>   |
|[<span data-ttu-id="ea049-113">Учет сотрудников</span><span class="sxs-lookup"><span data-stu-id="ea049-113">Post employees</span></span>](../api/dynamics-create-employee.md)  |<span data-ttu-id="ea049-114">сотрудников</span><span class="sxs-lookup"><span data-stu-id="ea049-114">employees</span></span>  |<span data-ttu-id="ea049-115">Создание объекта Employee.</span><span class="sxs-lookup"><span data-stu-id="ea049-115">Create an employee object.</span></span>|
|[<span data-ttu-id="ea049-116">Обновление сотрудников</span><span class="sxs-lookup"><span data-stu-id="ea049-116">Patch employees</span></span>](../api/dynamics-employee-update.md) |<span data-ttu-id="ea049-117">сотрудников</span><span class="sxs-lookup"><span data-stu-id="ea049-117">employees</span></span>  |<span data-ttu-id="ea049-118">Обновление объекта Employee.</span><span class="sxs-lookup"><span data-stu-id="ea049-118">Update an employee object.</span></span>|
|[<span data-ttu-id="ea049-119">Удаление сотрудников</span><span class="sxs-lookup"><span data-stu-id="ea049-119">Delete employees</span></span>](../api/dynamics-employee-delete.md)|<span data-ttu-id="ea049-120">Нет</span><span class="sxs-lookup"><span data-stu-id="ea049-120">none</span></span>       |<span data-ttu-id="ea049-121">Удаление объекта Employee.</span><span class="sxs-lookup"><span data-stu-id="ea049-121">Delete an employee object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ea049-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="ea049-122">Properties</span></span>
| <span data-ttu-id="ea049-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea049-123">Property</span></span>           | <span data-ttu-id="ea049-124">Тип</span><span class="sxs-lookup"><span data-stu-id="ea049-124">Type</span></span>   |<span data-ttu-id="ea049-125">Описание</span><span class="sxs-lookup"><span data-stu-id="ea049-125">Description</span></span>                                            |
|:-------------------|:-------|:------------------------------------------------------|
|<span data-ttu-id="ea049-126">id</span><span class="sxs-lookup"><span data-stu-id="ea049-126">id</span></span>                  |<span data-ttu-id="ea049-127">GUID</span><span class="sxs-lookup"><span data-stu-id="ea049-127">GUID</span></span>    |<span data-ttu-id="ea049-128">Идентификатор сотрудника.</span><span class="sxs-lookup"><span data-stu-id="ea049-128">The employee ID.</span></span> <span data-ttu-id="ea049-129">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="ea049-129">Non-editable.</span></span>                         |
|<span data-ttu-id="ea049-130">число</span><span class="sxs-lookup"><span data-stu-id="ea049-130">number</span></span>              |<span data-ttu-id="ea049-131">string</span><span class="sxs-lookup"><span data-stu-id="ea049-131">string</span></span>  |<span data-ttu-id="ea049-132">Номер сотрудника.</span><span class="sxs-lookup"><span data-stu-id="ea049-132">The employee number.</span></span> <span data-ttu-id="ea049-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ea049-133">Read-Only.</span></span>                        |
|<span data-ttu-id="ea049-134">displayName</span><span class="sxs-lookup"><span data-stu-id="ea049-134">displayName</span></span>         |<span data-ttu-id="ea049-135">string</span><span class="sxs-lookup"><span data-stu-id="ea049-135">string</span></span>  |<span data-ttu-id="ea049-136">Сотрудник givenName + фамилия.</span><span class="sxs-lookup"><span data-stu-id="ea049-136">The employee givenName + surname.</span></span> <span data-ttu-id="ea049-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ea049-137">Read-Only.</span></span>           |
|<span data-ttu-id="ea049-138">givenName;</span><span class="sxs-lookup"><span data-stu-id="ea049-138">givenName</span></span>           |<span data-ttu-id="ea049-139">string</span><span class="sxs-lookup"><span data-stu-id="ea049-139">string</span></span>  |<span data-ttu-id="ea049-140">Заданное имя сотрудника.</span><span class="sxs-lookup"><span data-stu-id="ea049-140">The given name of the employee.</span></span>                        |
|<span data-ttu-id="ea049-141">middleName</span><span class="sxs-lookup"><span data-stu-id="ea049-141">middleName</span></span>          |<span data-ttu-id="ea049-142">string</span><span class="sxs-lookup"><span data-stu-id="ea049-142">string</span></span>  |<span data-ttu-id="ea049-143">Отчество сотрудника.</span><span class="sxs-lookup"><span data-stu-id="ea049-143">The middle name of the employee.</span></span>                       |
|<span data-ttu-id="ea049-144">surname</span><span class="sxs-lookup"><span data-stu-id="ea049-144">surname</span></span>             |<span data-ttu-id="ea049-145">string</span><span class="sxs-lookup"><span data-stu-id="ea049-145">string</span></span>  |<span data-ttu-id="ea049-146">Фамилия сотрудника</span><span class="sxs-lookup"><span data-stu-id="ea049-146">The surname of the employee</span></span>                            |
|<span data-ttu-id="ea049-147">jobTitle;</span><span class="sxs-lookup"><span data-stu-id="ea049-147">jobTitle</span></span>            |<span data-ttu-id="ea049-148">string</span><span class="sxs-lookup"><span data-stu-id="ea049-148">string</span></span>  |<span data-ttu-id="ea049-149">Полное имя сотрудника</span><span class="sxs-lookup"><span data-stu-id="ea049-149">The full name of the employee</span></span>                          |
|<span data-ttu-id="ea049-150">address</span><span class="sxs-lookup"><span data-stu-id="ea049-150">address</span></span>             |[<span data-ttu-id="ea049-151">Навигационная. посталаддресс</span><span class="sxs-lookup"><span data-stu-id="ea049-151">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="ea049-152">Указывает адрес сотрудника.</span><span class="sxs-lookup"><span data-stu-id="ea049-152">Specifies the employee's address.</span></span> <span data-ttu-id="ea049-153">Этот адрес будет отображаться во всех документах ресурсов для сотрудника.</span><span class="sxs-lookup"><span data-stu-id="ea049-153">This address will appear on all resource documents for the employee.</span></span>|
|<span data-ttu-id="ea049-154">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="ea049-154">phoneNumber</span></span>         |<span data-ttu-id="ea049-155">string</span><span class="sxs-lookup"><span data-stu-id="ea049-155">string</span></span>  |<span data-ttu-id="ea049-156">Указывает номер телефона сотрудника.</span><span class="sxs-lookup"><span data-stu-id="ea049-156">Specifies the employee's telephone number.</span></span>             |
|<span data-ttu-id="ea049-157">mobilePhone;</span><span class="sxs-lookup"><span data-stu-id="ea049-157">mobilePhone</span></span>         |<span data-ttu-id="ea049-158">string</span><span class="sxs-lookup"><span data-stu-id="ea049-158">string</span></span>  |<span data-ttu-id="ea049-159">Указывает номер мобильного телефона сотрудника.</span><span class="sxs-lookup"><span data-stu-id="ea049-159">Specifies the employee's mobile telephone number.</span></span>      |
|<span data-ttu-id="ea049-160">email</span><span class="sxs-lookup"><span data-stu-id="ea049-160">email</span></span>               |<span data-ttu-id="ea049-161">строка</span><span class="sxs-lookup"><span data-stu-id="ea049-161">string</span></span>  |<span data-ttu-id="ea049-162">Указывает адрес электронной почты сотрудника.</span><span class="sxs-lookup"><span data-stu-id="ea049-162">Specifies the employee's email address.</span></span>                |
|<span data-ttu-id="ea049-163">персоналемаил</span><span class="sxs-lookup"><span data-stu-id="ea049-163">personalEmail</span></span>       |<span data-ttu-id="ea049-164">string</span><span class="sxs-lookup"><span data-stu-id="ea049-164">string</span></span>  |<span data-ttu-id="ea049-165">Указывает личный адрес электронной почты сотрудника.</span><span class="sxs-lookup"><span data-stu-id="ea049-165">Specifies the employee's personal email address.</span></span>       |
|<span data-ttu-id="ea049-166">емплойментдате</span><span class="sxs-lookup"><span data-stu-id="ea049-166">employmentDate</span></span>      |<span data-ttu-id="ea049-167">date</span><span class="sxs-lookup"><span data-stu-id="ea049-167">date</span></span>    |<span data-ttu-id="ea049-168">Указывает дату начала работы сотрудника в компании.</span><span class="sxs-lookup"><span data-stu-id="ea049-168">Specifies the date when the employee began to work for the company.</span></span>|
|<span data-ttu-id="ea049-169">терминатиондате</span><span class="sxs-lookup"><span data-stu-id="ea049-169">terminationDate</span></span>     |<span data-ttu-id="ea049-170">date</span><span class="sxs-lookup"><span data-stu-id="ea049-170">date</span></span>    |<span data-ttu-id="ea049-171">Указывает дату увольнения сотрудника, например из-за увольнения или увольнения.</span><span class="sxs-lookup"><span data-stu-id="ea049-171">Specifies the date when the employee was terminated, due to retirement or dismissal, for example.</span></span>|
|<span data-ttu-id="ea049-172">status</span><span class="sxs-lookup"><span data-stu-id="ea049-172">status</span></span>              |<span data-ttu-id="ea049-173">string</span><span class="sxs-lookup"><span data-stu-id="ea049-173">string</span></span>  |<span data-ttu-id="ea049-174">Указывает состояние сотрудника.</span><span class="sxs-lookup"><span data-stu-id="ea049-174">Specifies the employee's status.</span></span> <span data-ttu-id="ea049-175">Возможные значения: активные, неактивные или прерванные</span><span class="sxs-lookup"><span data-stu-id="ea049-175">Possible values are Active, Inactive or Terminated</span></span>|
|<span data-ttu-id="ea049-176">birthDate</span><span class="sxs-lookup"><span data-stu-id="ea049-176">birthDate</span></span>           |<span data-ttu-id="ea049-177">date</span><span class="sxs-lookup"><span data-stu-id="ea049-177">date</span></span>    |<span data-ttu-id="ea049-178">Указывает дату рождения сотрудника.</span><span class="sxs-lookup"><span data-stu-id="ea049-178">Specifies the employee's date of birth.</span></span>                |
|<span data-ttu-id="ea049-179">графические</span><span class="sxs-lookup"><span data-stu-id="ea049-179">picture</span></span>             |<span data-ttu-id="ea049-180">stream</span><span class="sxs-lookup"><span data-stu-id="ea049-180">stream</span></span>  |<span data-ttu-id="ea049-181">Фотография сотрудника.</span><span class="sxs-lookup"><span data-stu-id="ea049-181">The employee picture.</span></span> <span data-ttu-id="ea049-182">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ea049-182">Read-Only.</span></span>                       |
|<span data-ttu-id="ea049-183">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ea049-183">lastModifiedDateTime</span></span>|<span data-ttu-id="ea049-184">datetime</span><span class="sxs-lookup"><span data-stu-id="ea049-184">datetime</span></span>|<span data-ttu-id="ea049-185">Дата и время последнего изменения сотрудника.</span><span class="sxs-lookup"><span data-stu-id="ea049-185">The last datetime the employee was modified.</span></span> <span data-ttu-id="ea049-186">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ea049-186">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="ea049-187">Связи</span><span class="sxs-lookup"><span data-stu-id="ea049-187">Relationships</span></span>
<span data-ttu-id="ea049-188">Нет</span><span class="sxs-lookup"><span data-stu-id="ea049-188">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea049-189">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ea049-189">JSON representation</span></span>

<span data-ttu-id="ea049-190">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea049-190">Here is a JSON representation of the resource.</span></span>


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


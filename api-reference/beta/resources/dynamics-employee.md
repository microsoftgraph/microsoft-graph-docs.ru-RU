---
title: тип ресурса сотрудников
description: Объект сотрудника в Центре бизнеса Dynamics 365.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: eceea9e1811b61045c03fb8dc5d7710f33158ccc
ms.sourcegitcommit: a9a035e7cf7b500aebe5477c05361552e7c3a7ab
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/28/2021
ms.locfileid: "52695975"
---
# <a name="employees-resource-type"></a><span data-ttu-id="b2521-103">тип ресурса сотрудников</span><span class="sxs-lookup"><span data-stu-id="b2521-103">employees resource type</span></span>

<span data-ttu-id="b2521-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2521-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2521-105">Представляет сотрудника в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="b2521-105">Represents an employee in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="b2521-106">Методы</span><span class="sxs-lookup"><span data-stu-id="b2521-106">Methods</span></span>

| <span data-ttu-id="b2521-107">Метод</span><span class="sxs-lookup"><span data-stu-id="b2521-107">Method</span></span>                                              | <span data-ttu-id="b2521-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b2521-108">Return Type</span></span>|<span data-ttu-id="b2521-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b2521-109">Description</span></span>               |
|:----------------------------------------------------|:-----------|:-------------------------|
|[<span data-ttu-id="b2521-110">Получить сотрудников</span><span class="sxs-lookup"><span data-stu-id="b2521-110">Get employees</span></span>](../api/dynamics-employee-get.md)      |<span data-ttu-id="b2521-111">сотрудники</span><span class="sxs-lookup"><span data-stu-id="b2521-111">employees</span></span>  |<span data-ttu-id="b2521-112">Получите объект сотрудника.</span><span class="sxs-lookup"><span data-stu-id="b2521-112">Get an employee object.</span></span>   |
|[<span data-ttu-id="b2521-113">Почтовые сотрудники</span><span class="sxs-lookup"><span data-stu-id="b2521-113">Post employees</span></span>](../api/dynamics-create-employee.md)  |<span data-ttu-id="b2521-114">сотрудники</span><span class="sxs-lookup"><span data-stu-id="b2521-114">employees</span></span>  |<span data-ttu-id="b2521-115">Создание объекта сотрудника.</span><span class="sxs-lookup"><span data-stu-id="b2521-115">Create an employee object.</span></span>|
|[<span data-ttu-id="b2521-116">Сотрудники исправлений</span><span class="sxs-lookup"><span data-stu-id="b2521-116">Patch employees</span></span>](../api/dynamics-employee-update.md) |<span data-ttu-id="b2521-117">сотрудники</span><span class="sxs-lookup"><span data-stu-id="b2521-117">employees</span></span>  |<span data-ttu-id="b2521-118">Обновление объекта сотрудника.</span><span class="sxs-lookup"><span data-stu-id="b2521-118">Update an employee object.</span></span>|
|[<span data-ttu-id="b2521-119">Удаление сотрудников</span><span class="sxs-lookup"><span data-stu-id="b2521-119">Delete employees</span></span>](../api/dynamics-employee-delete.md)|<span data-ttu-id="b2521-120">нет</span><span class="sxs-lookup"><span data-stu-id="b2521-120">none</span></span>       |<span data-ttu-id="b2521-121">Удаление объекта сотрудника.</span><span class="sxs-lookup"><span data-stu-id="b2521-121">Delete an employee object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b2521-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2521-122">Properties</span></span>
| <span data-ttu-id="b2521-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2521-123">Property</span></span>           | <span data-ttu-id="b2521-124">Тип</span><span class="sxs-lookup"><span data-stu-id="b2521-124">Type</span></span>   |<span data-ttu-id="b2521-125">Описание</span><span class="sxs-lookup"><span data-stu-id="b2521-125">Description</span></span>                                            |
|:-------------------|:-------|:------------------------------------------------------|
|<span data-ttu-id="b2521-126">id</span><span class="sxs-lookup"><span data-stu-id="b2521-126">id</span></span>                  |<span data-ttu-id="b2521-127">GUID</span><span class="sxs-lookup"><span data-stu-id="b2521-127">GUID</span></span>    |<span data-ttu-id="b2521-128">ID сотрудника.</span><span class="sxs-lookup"><span data-stu-id="b2521-128">The employee ID.</span></span> <span data-ttu-id="b2521-129">Не редактируемый.</span><span class="sxs-lookup"><span data-stu-id="b2521-129">Non-editable.</span></span>                         |
|<span data-ttu-id="b2521-130">число</span><span class="sxs-lookup"><span data-stu-id="b2521-130">number</span></span>              |<span data-ttu-id="b2521-131">string</span><span class="sxs-lookup"><span data-stu-id="b2521-131">string</span></span>  |<span data-ttu-id="b2521-132">Номер сотрудника.</span><span class="sxs-lookup"><span data-stu-id="b2521-132">The employee number.</span></span> <span data-ttu-id="b2521-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b2521-133">Read-Only.</span></span>                        |
|<span data-ttu-id="b2521-134">displayName</span><span class="sxs-lookup"><span data-stu-id="b2521-134">displayName</span></span>         |<span data-ttu-id="b2521-135">string</span><span class="sxs-lookup"><span data-stu-id="b2521-135">string</span></span>  |<span data-ttu-id="b2521-136">Сотрудник, задав имя + фамилию.</span><span class="sxs-lookup"><span data-stu-id="b2521-136">The employee givenName + surname.</span></span> <span data-ttu-id="b2521-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b2521-137">Read-Only.</span></span>           |
|<span data-ttu-id="b2521-138">givenName</span><span class="sxs-lookup"><span data-stu-id="b2521-138">givenName</span></span>           |<span data-ttu-id="b2521-139">string</span><span class="sxs-lookup"><span data-stu-id="b2521-139">string</span></span>  |<span data-ttu-id="b2521-140">Заданное имя сотрудника.</span><span class="sxs-lookup"><span data-stu-id="b2521-140">The given name of the employee.</span></span>                        |
|<span data-ttu-id="b2521-141">middleName</span><span class="sxs-lookup"><span data-stu-id="b2521-141">middleName</span></span>          |<span data-ttu-id="b2521-142">string</span><span class="sxs-lookup"><span data-stu-id="b2521-142">string</span></span>  |<span data-ttu-id="b2521-143">Среднее имя сотрудника.</span><span class="sxs-lookup"><span data-stu-id="b2521-143">The middle name of the employee.</span></span>                       |
|<span data-ttu-id="b2521-144">surname</span><span class="sxs-lookup"><span data-stu-id="b2521-144">surname</span></span>             |<span data-ttu-id="b2521-145">string</span><span class="sxs-lookup"><span data-stu-id="b2521-145">string</span></span>  |<span data-ttu-id="b2521-146">Фамилия сотрудника</span><span class="sxs-lookup"><span data-stu-id="b2521-146">The surname of the employee</span></span>                            |
|<span data-ttu-id="b2521-147">jobTitle;</span><span class="sxs-lookup"><span data-stu-id="b2521-147">jobTitle</span></span>            |<span data-ttu-id="b2521-148">string</span><span class="sxs-lookup"><span data-stu-id="b2521-148">string</span></span>  |<span data-ttu-id="b2521-149">Название задания сотрудника</span><span class="sxs-lookup"><span data-stu-id="b2521-149">The job title of the employee</span></span>                          |
|<span data-ttu-id="b2521-150">address</span><span class="sxs-lookup"><span data-stu-id="b2521-150">address</span></span>             |[<span data-ttu-id="b2521-151">NAV. PostalAddress</span><span class="sxs-lookup"><span data-stu-id="b2521-151">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="b2521-152">Указывает адрес сотрудника.</span><span class="sxs-lookup"><span data-stu-id="b2521-152">Specifies the employee's address.</span></span> <span data-ttu-id="b2521-153">Этот адрес будет отображаться во всех документах ресурса для сотрудника.</span><span class="sxs-lookup"><span data-stu-id="b2521-153">This address will appear on all resource documents for the employee.</span></span>|
|<span data-ttu-id="b2521-154">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="b2521-154">phoneNumber</span></span>         |<span data-ttu-id="b2521-155">string</span><span class="sxs-lookup"><span data-stu-id="b2521-155">string</span></span>  |<span data-ttu-id="b2521-156">Указывает телефонный номер сотрудника.</span><span class="sxs-lookup"><span data-stu-id="b2521-156">Specifies the employee's telephone number.</span></span>             |
|<span data-ttu-id="b2521-157">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="b2521-157">mobilePhone</span></span>         |<span data-ttu-id="b2521-158">string</span><span class="sxs-lookup"><span data-stu-id="b2521-158">string</span></span>  |<span data-ttu-id="b2521-159">Указывает номер мобильного телефона сотрудника.</span><span class="sxs-lookup"><span data-stu-id="b2521-159">Specifies the employee's mobile telephone number.</span></span>      |
|<span data-ttu-id="b2521-160">email</span><span class="sxs-lookup"><span data-stu-id="b2521-160">email</span></span>               |<span data-ttu-id="b2521-161">строка</span><span class="sxs-lookup"><span data-stu-id="b2521-161">string</span></span>  |<span data-ttu-id="b2521-162">Указывает адрес электронной почты сотрудника.</span><span class="sxs-lookup"><span data-stu-id="b2521-162">Specifies the employee's email address.</span></span>                |
|<span data-ttu-id="b2521-163">personalEmail</span><span class="sxs-lookup"><span data-stu-id="b2521-163">personalEmail</span></span>       |<span data-ttu-id="b2521-164">string</span><span class="sxs-lookup"><span data-stu-id="b2521-164">string</span></span>  |<span data-ttu-id="b2521-165">Указывает личный адрес электронной почты сотрудника.</span><span class="sxs-lookup"><span data-stu-id="b2521-165">Specifies the employee's personal email address.</span></span>       |
|<span data-ttu-id="b2521-166">employmentDate</span><span class="sxs-lookup"><span data-stu-id="b2521-166">employmentDate</span></span>      |<span data-ttu-id="b2521-167">date</span><span class="sxs-lookup"><span data-stu-id="b2521-167">date</span></span>    |<span data-ttu-id="b2521-168">Указывает дату начала работы сотрудника в компании.</span><span class="sxs-lookup"><span data-stu-id="b2521-168">Specifies the date when the employee began to work for the company.</span></span>|
|<span data-ttu-id="b2521-169">terminationDate</span><span class="sxs-lookup"><span data-stu-id="b2521-169">terminationDate</span></span>     |<span data-ttu-id="b2521-170">date</span><span class="sxs-lookup"><span data-stu-id="b2521-170">date</span></span>    |<span data-ttu-id="b2521-171">Указывает дату, когда сотрудник был уволен, например в связи с выходом на пенсию или увольнением.</span><span class="sxs-lookup"><span data-stu-id="b2521-171">Specifies the date when the employee was terminated, due to retirement or dismissal, for example.</span></span>|
|<span data-ttu-id="b2521-172">status</span><span class="sxs-lookup"><span data-stu-id="b2521-172">status</span></span>              |<span data-ttu-id="b2521-173">string</span><span class="sxs-lookup"><span data-stu-id="b2521-173">string</span></span>  |<span data-ttu-id="b2521-174">Указывает состояние сотрудника.</span><span class="sxs-lookup"><span data-stu-id="b2521-174">Specifies the employee's status.</span></span> <span data-ttu-id="b2521-175">Возможные значения Active, Inactive или Terminated</span><span class="sxs-lookup"><span data-stu-id="b2521-175">Possible values are Active, Inactive or Terminated</span></span>|
|<span data-ttu-id="b2521-176">birthDate</span><span class="sxs-lookup"><span data-stu-id="b2521-176">birthDate</span></span>           |<span data-ttu-id="b2521-177">date</span><span class="sxs-lookup"><span data-stu-id="b2521-177">date</span></span>    |<span data-ttu-id="b2521-178">Указывает дату рождения сотрудника.</span><span class="sxs-lookup"><span data-stu-id="b2521-178">Specifies the employee's date of birth.</span></span>                |
|<span data-ttu-id="b2521-179">изображение</span><span class="sxs-lookup"><span data-stu-id="b2521-179">picture</span></span>             |<span data-ttu-id="b2521-180">stream</span><span class="sxs-lookup"><span data-stu-id="b2521-180">stream</span></span>  |<span data-ttu-id="b2521-181">Изображение сотрудника.</span><span class="sxs-lookup"><span data-stu-id="b2521-181">The employee picture.</span></span> <span data-ttu-id="b2521-182">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b2521-182">Read-Only.</span></span>                       |
|<span data-ttu-id="b2521-183">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b2521-183">lastModifiedDateTime</span></span>|<span data-ttu-id="b2521-184">datetime</span><span class="sxs-lookup"><span data-stu-id="b2521-184">datetime</span></span>|<span data-ttu-id="b2521-185">В последний раз сотрудник был изменен.</span><span class="sxs-lookup"><span data-stu-id="b2521-185">The last datetime the employee was modified.</span></span> <span data-ttu-id="b2521-186">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b2521-186">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="b2521-187">Связи</span><span class="sxs-lookup"><span data-stu-id="b2521-187">Relationships</span></span>
<span data-ttu-id="b2521-188">Нет</span><span class="sxs-lookup"><span data-stu-id="b2521-188">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2521-189">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2521-189">JSON representation</span></span>

<span data-ttu-id="b2521-190">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2521-190">Here is a JSON representation of the resource.</span></span>


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




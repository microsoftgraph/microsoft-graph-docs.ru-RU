---
title: тип перечисления Граупполициоператионтипе
description: Тип операции с групповой политикой.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3319ddb45c59a829b3275b889aa54a4f8ec4bb8b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49259657"
---
# <a name="grouppolicyoperationtype-enum-type"></a><span data-ttu-id="fa4a8-103">тип перечисления Граупполициоператионтипе</span><span class="sxs-lookup"><span data-stu-id="fa4a8-103">groupPolicyOperationType enum type</span></span>

<span data-ttu-id="fa4a8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa4a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fa4a8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa4a8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa4a8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fa4a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa4a8-107">Тип операции с групповой политикой.</span><span class="sxs-lookup"><span data-stu-id="fa4a8-107">Type of Group Policy operation.</span></span>

## <a name="members"></a><span data-ttu-id="fa4a8-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="fa4a8-108">Members</span></span>
|<span data-ttu-id="fa4a8-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="fa4a8-109">Member</span></span>|<span data-ttu-id="fa4a8-110">Значение</span><span class="sxs-lookup"><span data-stu-id="fa4a8-110">Value</span></span>|<span data-ttu-id="fa4a8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fa4a8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa4a8-112">Нет</span><span class="sxs-lookup"><span data-stu-id="fa4a8-112">none</span></span>|<span data-ttu-id="fa4a8-113">нуль</span><span class="sxs-lookup"><span data-stu-id="fa4a8-113">0</span></span>|<span data-ttu-id="fa4a8-114">Групповая политика: недопустимый тип операции.</span><span class="sxs-lookup"><span data-stu-id="fa4a8-114">Group Policy invalid operation type.</span></span>|
|<span data-ttu-id="fa4a8-115">загрузку</span><span class="sxs-lookup"><span data-stu-id="fa4a8-115">upload</span></span>|<span data-ttu-id="fa4a8-116">1,1</span><span class="sxs-lookup"><span data-stu-id="fa4a8-116">1</span></span>|<span data-ttu-id="fa4a8-117">Тип операции отправки групповой политики.</span><span class="sxs-lookup"><span data-stu-id="fa4a8-117">Group Policy upload operation type.</span></span>|
|<span data-ttu-id="fa4a8-118">уплоадневверсион</span><span class="sxs-lookup"><span data-stu-id="fa4a8-118">uploadNewVersion</span></span>|<span data-ttu-id="fa4a8-119">2</span><span class="sxs-lookup"><span data-stu-id="fa4a8-119">2</span></span>|<span data-ttu-id="fa4a8-120">Отправка типа операции новой версии групповой политики.</span><span class="sxs-lookup"><span data-stu-id="fa4a8-120">Group Policy upload new version operation type.</span></span>|
|<span data-ttu-id="fa4a8-121">аддлангуажефилес</span><span class="sxs-lookup"><span data-stu-id="fa4a8-121">addLanguageFiles</span></span>|<span data-ttu-id="fa4a8-122">4</span><span class="sxs-lookup"><span data-stu-id="fa4a8-122">3</span></span>|<span data-ttu-id="fa4a8-123">Тип операции "Добавление файлов нового языка" групповой политики (ADML).</span><span class="sxs-lookup"><span data-stu-id="fa4a8-123">Group Policy add new language(ADML) files operation type.</span></span>|
|<span data-ttu-id="fa4a8-124">ремовелангуажефилес</span><span class="sxs-lookup"><span data-stu-id="fa4a8-124">removeLanguageFiles</span></span>|<span data-ttu-id="fa4a8-125">4 </span><span class="sxs-lookup"><span data-stu-id="fa4a8-125">4</span></span>|<span data-ttu-id="fa4a8-126">Тип операции удаления файлов на языке групповой политики (ADML).</span><span class="sxs-lookup"><span data-stu-id="fa4a8-126">Group Policy remove language(ADML) files operation type.</span></span>|
|<span data-ttu-id="fa4a8-127">упдателангуажефилес</span><span class="sxs-lookup"><span data-stu-id="fa4a8-127">updateLanguageFiles</span></span>|<span data-ttu-id="fa4a8-128">5 </span><span class="sxs-lookup"><span data-stu-id="fa4a8-128">5</span></span>|<span data-ttu-id="fa4a8-129">Тип операции для файлов на языке обновлений групповой политики (ADML).</span><span class="sxs-lookup"><span data-stu-id="fa4a8-129">Group Policy update language(ADML) files operation type.</span></span>|
|<span data-ttu-id="fa4a8-130">удалить</span><span class="sxs-lookup"><span data-stu-id="fa4a8-130">remove</span></span>|<span data-ttu-id="fa4a8-131">6 </span><span class="sxs-lookup"><span data-stu-id="fa4a8-131">6</span></span>|<span data-ttu-id="fa4a8-132">Групповая политика удалить отправленный тип операции с файлами.</span><span class="sxs-lookup"><span data-stu-id="fa4a8-132">Group Policy remove uploaded file operation type.</span></span>|





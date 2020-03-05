---
title: Тип ресурса Profile
description: Представляет свойства, которые являются описательными для пользователя и представлены в общедоступных людях в Microsoft 365 и службах и возможностях сторонних производителей с помощью Microsoft Graph.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: c5c7d7765d546dad5f6de39f72f092b3bf9daee6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521469"
---
# <a name="profile-resource-type"></a><span data-ttu-id="f1c0e-103">Тип ресурса Profile</span><span class="sxs-lookup"><span data-stu-id="f1c0e-103">profile resource type</span></span>

<span data-ttu-id="f1c0e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f1c0e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1c0e-105">Представляет свойства описания человека в клиенте.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-105">Represents descriptive properties of a person in a tenant.</span></span> <span data-ttu-id="f1c0e-106">Эти свойства отображаются в общедоступных людях в Microsoft 365 и сторонних службах и возможностях в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-106">These properties are surfaced in shared people experiences across Microsoft 365 and third-party services and experiences via Microsoft Graph.</span></span> 

## <a name="methods"></a><span data-ttu-id="f1c0e-107">Методы</span><span class="sxs-lookup"><span data-stu-id="f1c0e-107">Methods</span></span>

| <span data-ttu-id="f1c0e-108">Метод</span><span class="sxs-lookup"><span data-stu-id="f1c0e-108">Method</span></span>                                                                     | <span data-ttu-id="f1c0e-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f1c0e-109">Return Type</span></span>                                                    | <span data-ttu-id="f1c0e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f1c0e-110">Description</span></span>                                                                          |
|:---------------------------------------------------------------------------|:---------------------------------------------------------------|:-------------------------------------------------------------------------------------|
| [<span data-ttu-id="f1c0e-111">Получение профиля</span><span class="sxs-lookup"><span data-stu-id="f1c0e-111">Get profile</span></span>](../api/profile-get.md)                                       | [<span data-ttu-id="f1c0e-112">profile</span><span class="sxs-lookup"><span data-stu-id="f1c0e-112">profile</span></span>](profile.md)                                          | <span data-ttu-id="f1c0e-113">Чтение свойств и связей объекта Profile.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-113">Read properties and relationships of profile object.</span></span>                                 |
| [<span data-ttu-id="f1c0e-114">Удаление профиля</span><span class="sxs-lookup"><span data-stu-id="f1c0e-114">Delete profile</span></span>](../api/profile-delete.md)                                         | <span data-ttu-id="f1c0e-115">Нет</span><span class="sxs-lookup"><span data-stu-id="f1c0e-115">None</span></span>                                                           | <span data-ttu-id="f1c0e-116">Удаление объекта **Profile** .</span><span class="sxs-lookup"><span data-stu-id="f1c0e-116">Delete a **profile** object.</span></span>                                                               |
| [<span data-ttu-id="f1c0e-117">Учетная запись списка</span><span class="sxs-lookup"><span data-stu-id="f1c0e-117">List account</span></span>](../api/profile-list-account.md)                             | <span data-ttu-id="f1c0e-118">Коллекция [усераккаунтинформатион](useraccountinformation.md)</span><span class="sxs-lookup"><span data-stu-id="f1c0e-118">[userAccountInformation](useraccountinformation.md) collection</span></span> | <span data-ttu-id="f1c0e-119">Получение коллекции объектов **усераккаунтинформатион** .</span><span class="sxs-lookup"><span data-stu-id="f1c0e-119">Get a **userAccountInformation** object collection.</span></span>                                      |
| [<span data-ttu-id="f1c0e-120">Создание Персонанниверсари</span><span class="sxs-lookup"><span data-stu-id="f1c0e-120">Create personAnniversary</span></span>](../api/profile-post-anniversaries.md)           | [<span data-ttu-id="f1c0e-121">персонанниверсари</span><span class="sxs-lookup"><span data-stu-id="f1c0e-121">personAnniversary</span></span>](personanniversary.md)                      | <span data-ttu-id="f1c0e-122">Создание нового **персонанниверсари** путем публикации в коллекции юбилеев.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-122">Create a new **personAnniversary** by posting to the anniversaries collection.</span></span>           |
| [<span data-ttu-id="f1c0e-123">Список юбилеев</span><span class="sxs-lookup"><span data-stu-id="f1c0e-123">List anniversaries</span></span>](../api/profile-list-anniversaries.md)                 | <span data-ttu-id="f1c0e-124">Коллекция [персонанниверсари](personanniversary.md)</span><span class="sxs-lookup"><span data-stu-id="f1c0e-124">[personAnniversary](personanniversary.md) collection</span></span>           | <span data-ttu-id="f1c0e-125">Получение коллекции объектов **персонанниверсари** .</span><span class="sxs-lookup"><span data-stu-id="f1c0e-125">Get a **personAnniversary** object collection.</span></span>                                           |
| [<span data-ttu-id="f1c0e-126">Создание Едукатионалактивити</span><span class="sxs-lookup"><span data-stu-id="f1c0e-126">Create educationalActivity</span></span>](../api/profile-post-educationalactivities.md) | [<span data-ttu-id="f1c0e-127">едукатионалактивити</span><span class="sxs-lookup"><span data-stu-id="f1c0e-127">educationalActivity</span></span>](educationalactivity.md)                  | <span data-ttu-id="f1c0e-128">Создание нового **едукатионалактивити** путем отправки в коллекцию **едукатионалактивитиес** .</span><span class="sxs-lookup"><span data-stu-id="f1c0e-128">Create a new **educationalActivity** by posting to the **educationalActivities** collection.</span></span> |
| [<span data-ttu-id="f1c0e-129">Список Едукатионалактивитиес</span><span class="sxs-lookup"><span data-stu-id="f1c0e-129">List educationalActivities</span></span>](../api/profile-list-educationalactivities.md) | <span data-ttu-id="f1c0e-130">Коллекция [едукатионалактивити](educationalactivity.md)</span><span class="sxs-lookup"><span data-stu-id="f1c0e-130">[educationalActivity](educationalactivity.md) collection</span></span>       | <span data-ttu-id="f1c0e-131">Получение коллекции объектов **едукатионалактивити** .</span><span class="sxs-lookup"><span data-stu-id="f1c0e-131">Get an **educationalActivity** object collection.</span></span>                                         |
| [<span data-ttu-id="f1c0e-132">Создание Итемемаил</span><span class="sxs-lookup"><span data-stu-id="f1c0e-132">Create itemEmail</span></span>](../api/profile-post-emails.md)                          | [<span data-ttu-id="f1c0e-133">итемемаил</span><span class="sxs-lookup"><span data-stu-id="f1c0e-133">itemEmail</span></span>](itememail.md)                                      | <span data-ttu-id="f1c0e-134">Создание нового **итемемаил** путем отправки в коллекцию сообщений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-134">Create a new **itemEmail** by posting to the emails collection.</span></span>                          |
| [<span data-ttu-id="f1c0e-135">Список сообщений электронной почты</span><span class="sxs-lookup"><span data-stu-id="f1c0e-135">List emails</span></span>](../api/profile-list-emails.md)                               | <span data-ttu-id="f1c0e-136">Коллекция [итемемаил](itememail.md)</span><span class="sxs-lookup"><span data-stu-id="f1c0e-136">[itemEmail](itememail.md) collection</span></span>                           | <span data-ttu-id="f1c0e-137">Получение коллекции объектов **итемемаил** .</span><span class="sxs-lookup"><span data-stu-id="f1c0e-137">Get an **itemEmail** object collection.</span></span>                                                   |
| [<span data-ttu-id="f1c0e-138">Создание Персонинтерест</span><span class="sxs-lookup"><span data-stu-id="f1c0e-138">Create personInterest</span></span>](../api/profile-post-interests.md)                  | [<span data-ttu-id="f1c0e-139">персонинтерест</span><span class="sxs-lookup"><span data-stu-id="f1c0e-139">personInterest</span></span>](personinterest.md)                            | <span data-ttu-id="f1c0e-140">Создание нового **персонинтерест** путем отправки в коллекцию интересов.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-140">Create a new **personInterest** by posting to the interests collection.</span></span>                  |
| [<span data-ttu-id="f1c0e-141">Список интересов</span><span class="sxs-lookup"><span data-stu-id="f1c0e-141">List interests</span></span>](../api/profile-list-interests.md)                         | <span data-ttu-id="f1c0e-142">Коллекция [персонинтерест](personinterest.md)</span><span class="sxs-lookup"><span data-stu-id="f1c0e-142">[personInterest](personinterest.md) collection</span></span>                 | <span data-ttu-id="f1c0e-143">Получение коллекции объектов **персонинтерест** .</span><span class="sxs-lookup"><span data-stu-id="f1c0e-143">Get a **personInterest** object collection.</span></span>                                              |
| [<span data-ttu-id="f1c0e-144">Создание ЛангуажепрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="f1c0e-144">Create languageProficiency</span></span>](../api/profile-post-languages.md)             | [<span data-ttu-id="f1c0e-145">лангуажепрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="f1c0e-145">languageProficiency</span></span>](languageproficiency.md)                  | <span data-ttu-id="f1c0e-146">Создание нового **лангуажепрофиЦиенци** путем публикации в коллекции Languages.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-146">Create a new **languageProficiency** by posting to the languages collection.</span></span>             |
| [<span data-ttu-id="f1c0e-147">Список языков</span><span class="sxs-lookup"><span data-stu-id="f1c0e-147">List languages</span></span>](../api/profile-list-languages.md)                         | <span data-ttu-id="f1c0e-148">Коллекция [лангуажепрофиЦиенци](languageproficiency.md)</span><span class="sxs-lookup"><span data-stu-id="f1c0e-148">[languageProficiency](languageproficiency.md) collection</span></span>       | <span data-ttu-id="f1c0e-149">Получение коллекции объектов **лангуажепрофиЦиенци** .</span><span class="sxs-lookup"><span data-stu-id="f1c0e-149">Get a **languageProficiency** object collection.</span></span>                                         |
| [<span data-ttu-id="f1c0e-150">Список имен</span><span class="sxs-lookup"><span data-stu-id="f1c0e-150">List names</span></span>](../api/profile-list-names.md)                                 | <span data-ttu-id="f1c0e-151">Коллекция [PersonName](personname.md)</span><span class="sxs-lookup"><span data-stu-id="f1c0e-151">[personName](personname.md) collection</span></span>                         | <span data-ttu-id="f1c0e-152">Получение коллекции объектов **PersonName** .</span><span class="sxs-lookup"><span data-stu-id="f1c0e-152">Get a **personName** object collection.</span></span>                                                  |
| [<span data-ttu-id="f1c0e-153">Создание personName</span><span class="sxs-lookup"><span data-stu-id="f1c0e-153">Create personName</span></span>](../api/profile-post-names.md)                          | [<span data-ttu-id="f1c0e-154">personName</span><span class="sxs-lookup"><span data-stu-id="f1c0e-154">personName</span></span>](personName.md)                                    | <span data-ttu-id="f1c0e-155">Создайте новый объект **PersonName** , отправив его в коллекцию Names.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-155">Create a new **personName** object by posting to the names collection.</span></span>                   |
| [<span data-ttu-id="f1c0e-156">Список веб-сайтов</span><span class="sxs-lookup"><span data-stu-id="f1c0e-156">List websites</span></span>](../api/profile-list-websites.md)                           | <span data-ttu-id="f1c0e-157">Коллекция [персонвебсите](personwebsite.md)</span><span class="sxs-lookup"><span data-stu-id="f1c0e-157">[personWebsite](personwebsite.md) collection</span></span>                   | <span data-ttu-id="f1c0e-158">Получение коллекции объектов **персонвебсите** .</span><span class="sxs-lookup"><span data-stu-id="f1c0e-158">Get a **personWebsite** object collection.</span></span>                                               |
| [<span data-ttu-id="f1c0e-159">Создание Итемфоне</span><span class="sxs-lookup"><span data-stu-id="f1c0e-159">Create itemPhone</span></span>](../api/profile-post-phones.md)                          | [<span data-ttu-id="f1c0e-160">итемфоне</span><span class="sxs-lookup"><span data-stu-id="f1c0e-160">itemPhone</span></span>](itemphone.md)                                      | <span data-ttu-id="f1c0e-161">Создание нового Итемфоне путем публикации в коллекции phones.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-161">Create a new itemPhone by posting to the phones collection.</span></span>                          |
| [<span data-ttu-id="f1c0e-162">Перечисление телефонов</span><span class="sxs-lookup"><span data-stu-id="f1c0e-162">List phones</span></span>](../api/profile-list-phones.md)                               | <span data-ttu-id="f1c0e-163">Коллекция [итемфоне](itemphone.md)</span><span class="sxs-lookup"><span data-stu-id="f1c0e-163">[itemPhone](itemphone.md) collection</span></span>                           | <span data-ttu-id="f1c0e-164">Получение коллекции объектов **итемфоне** .</span><span class="sxs-lookup"><span data-stu-id="f1c0e-164">Get a **itemPhone** object collection.</span></span>                                                   |
| [<span data-ttu-id="f1c0e-165">Создание Воркпоситион</span><span class="sxs-lookup"><span data-stu-id="f1c0e-165">Create workPosition</span></span>](../api/profile-post-positions.md)                    | [<span data-ttu-id="f1c0e-166">воркпоситион</span><span class="sxs-lookup"><span data-stu-id="f1c0e-166">workPosition</span></span>](workposition.md)                                | <span data-ttu-id="f1c0e-167">Создание нового Воркпоситион путем отправки в коллекцию Positions.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-167">Create a new workPosition by posting to the positions collection.</span></span>                    |
| [<span data-ttu-id="f1c0e-168">Позиции списка</span><span class="sxs-lookup"><span data-stu-id="f1c0e-168">List positions</span></span>](../api/profile-list-positions.md)                         | <span data-ttu-id="f1c0e-169">Коллекция [воркпоситион](workposition.md)</span><span class="sxs-lookup"><span data-stu-id="f1c0e-169">[workPosition](workposition.md) collection</span></span>                     | <span data-ttu-id="f1c0e-170">Получение коллекции объектов **воркпоситион** .</span><span class="sxs-lookup"><span data-stu-id="f1c0e-170">Get a **workPosition** object collection.</span></span>                                                |
| [<span data-ttu-id="f1c0e-171">Создание ПрожектпартиЦипатион</span><span class="sxs-lookup"><span data-stu-id="f1c0e-171">Create projectParticipation</span></span>](../api/profile-post-projects.md)             | [<span data-ttu-id="f1c0e-172">прожектпартиЦипатион</span><span class="sxs-lookup"><span data-stu-id="f1c0e-172">projectParticipation</span></span>](projectparticipation.md)                | <span data-ttu-id="f1c0e-173">Создание нового **прожектпартиЦипатион** путем публикации в коллекции проектов.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-173">Create a new **projectParticipation** by posting to the projects collection.</span></span>             |
| [<span data-ttu-id="f1c0e-174">Список проектов</span><span class="sxs-lookup"><span data-stu-id="f1c0e-174">List projects</span></span>](../api/profile-list-projects.md)                           | <span data-ttu-id="f1c0e-175">Коллекция [прожектпартиЦипатион](projectparticipation.md)</span><span class="sxs-lookup"><span data-stu-id="f1c0e-175">[projectParticipation](projectparticipation.md) collection</span></span>     | <span data-ttu-id="f1c0e-176">Получение коллекции объектов **прожектпартиЦипатион** .</span><span class="sxs-lookup"><span data-stu-id="f1c0e-176">Get a **projectParticipation** object collection.</span></span>                                        |
| [<span data-ttu-id="f1c0e-177">Создание СкиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="f1c0e-177">Create skillProficiency</span></span>](../api/profile-post-skills.md)                   | [<span data-ttu-id="f1c0e-178">скиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="f1c0e-178">skillProficiency</span></span>](skillproficiency.md)                        | <span data-ttu-id="f1c0e-179">Создание нового **скиллпрофиЦиенци** путем публикации в коллекции навыков.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-179">Create a new **skillProficiency** by posting to the skills collection.</span></span>                   |
| [<span data-ttu-id="f1c0e-180">Список навыков</span><span class="sxs-lookup"><span data-stu-id="f1c0e-180">List skills</span></span>](../api/profile-list-skills.md)                               | <span data-ttu-id="f1c0e-181">Коллекция [скиллпрофиЦиенци](skillproficiency.md)</span><span class="sxs-lookup"><span data-stu-id="f1c0e-181">[skillProficiency](skillproficiency.md) collection</span></span>             | <span data-ttu-id="f1c0e-182">Получение коллекции объектов **скиллпрофиЦиенци** .</span><span class="sxs-lookup"><span data-stu-id="f1c0e-182">Get a **skillProficiency** object collection.</span></span>                                            |
| [<span data-ttu-id="f1c0e-183">Создание учетной записи</span><span class="sxs-lookup"><span data-stu-id="f1c0e-183">Create webAccount</span></span>](../api/profile-post-webaccounts.md)                    | [<span data-ttu-id="f1c0e-184">Учетная запись учетной записи</span><span class="sxs-lookup"><span data-stu-id="f1c0e-184">webAccount</span></span>](webaccount.md)                                    | <span data-ttu-id="f1c0e-185">Создайте новую **учетную запись** , разместив ее в коллекции учетных записей.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-185">Create a new **webAccount** by posting to the webAccounts collection.</span></span>                    |
| [<span data-ttu-id="f1c0e-186">Список учетных записей</span><span class="sxs-lookup"><span data-stu-id="f1c0e-186">List webAccounts</span></span>](../api/profile-list-webaccounts.md)                     | <span data-ttu-id="f1c0e-187">Коллекция [учетных записей](webaccount.md)</span><span class="sxs-lookup"><span data-stu-id="f1c0e-187">[webAccount](webaccount.md) collection</span></span>                         | <span data-ttu-id="f1c0e-188">Получение коллекции объектов **учетных записей** .</span><span class="sxs-lookup"><span data-stu-id="f1c0e-188">Get a **webAccount** object collection.</span></span>                                                  |
| [<span data-ttu-id="f1c0e-189">Создание Персонвебсите</span><span class="sxs-lookup"><span data-stu-id="f1c0e-189">Create personWebsite</span></span>](../api/profile-post-websites.md)                    | [<span data-ttu-id="f1c0e-190">персонвебсите</span><span class="sxs-lookup"><span data-stu-id="f1c0e-190">personWebsite</span></span>](personwebsite.md)                              | <span data-ttu-id="f1c0e-191">Создание нового **персонвебсите** путем публикации в семействе веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-191">Create a new **personWebsite** by posting to the websites collection.</span></span>                    |
| [<span data-ttu-id="f1c0e-192">Список веб-сайтов</span><span class="sxs-lookup"><span data-stu-id="f1c0e-192">List websites</span></span>](../api/profile-list-websites.md)                           | <span data-ttu-id="f1c0e-193">Коллекция [персонвебсите](personwebsite.md)</span><span class="sxs-lookup"><span data-stu-id="f1c0e-193">[personWebsite](personwebsite.md) collection</span></span>                   | <span data-ttu-id="f1c0e-194">Получение коллекции объектов **персонвебсите** .</span><span class="sxs-lookup"><span data-stu-id="f1c0e-194">Get a **personWebsite** object collection.</span></span>                                               |

## <a name="properties"></a><span data-ttu-id="f1c0e-195">Свойства</span><span class="sxs-lookup"><span data-stu-id="f1c0e-195">Properties</span></span>

| <span data-ttu-id="f1c0e-196">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1c0e-196">Property</span></span>     | <span data-ttu-id="f1c0e-197">Тип</span><span class="sxs-lookup"><span data-stu-id="f1c0e-197">Type</span></span>        | <span data-ttu-id="f1c0e-198">Описание</span><span class="sxs-lookup"><span data-stu-id="f1c0e-198">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f1c0e-199">id</span><span class="sxs-lookup"><span data-stu-id="f1c0e-199">id</span></span>            |<span data-ttu-id="f1c0e-200">String</span><span class="sxs-lookup"><span data-stu-id="f1c0e-200">String</span></span>       | <span data-ttu-id="f1c0e-201">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-201">Read-only.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="f1c0e-202">Отношения</span><span class="sxs-lookup"><span data-stu-id="f1c0e-202">Relationships</span></span>

| <span data-ttu-id="f1c0e-203">Связь</span><span class="sxs-lookup"><span data-stu-id="f1c0e-203">Relationship</span></span>          | <span data-ttu-id="f1c0e-204">Тип</span><span class="sxs-lookup"><span data-stu-id="f1c0e-204">Type</span></span>                                                         | <span data-ttu-id="f1c0e-205">Описание</span><span class="sxs-lookup"><span data-stu-id="f1c0e-205">Description</span></span>         |
|:----------------------|:-------------------------------------------------------------|:--------------------|
|<span data-ttu-id="f1c0e-206">финансового</span><span class="sxs-lookup"><span data-stu-id="f1c0e-206">account</span></span>                |<span data-ttu-id="f1c0e-207">Коллекция [усераккаунтинформатион](useraccountinformation.md)</span><span class="sxs-lookup"><span data-stu-id="f1c0e-207">[userAccountInformation](useraccountinformation.md) collection</span></span>| <span data-ttu-id="f1c0e-208">Представляет сведения, специально связанные с учетной записью пользователя.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-208">Represents information specifically tied to a user's account.</span></span> <span data-ttu-id="f1c0e-209">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-209">Read-only.</span></span> <span data-ttu-id="f1c0e-210">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-210">Nullable.</span></span>|
|<span data-ttu-id="f1c0e-211">годовщины</span><span class="sxs-lookup"><span data-stu-id="f1c0e-211">anniversaries</span></span>          |<span data-ttu-id="f1c0e-212">Коллекция [персонанниверсари](personanniversary.md)</span><span class="sxs-lookup"><span data-stu-id="f1c0e-212">[personAnniversary](personanniversary.md) collection</span></span>          | <span data-ttu-id="f1c0e-213">Представляет сведения о значимых датах, связанных с пользователем.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-213">Represents the details of meaningful dates associated with a person.</span></span> <span data-ttu-id="f1c0e-214">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-214">Read-only.</span></span> <span data-ttu-id="f1c0e-215">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-215">Nullable.</span></span>|
|<span data-ttu-id="f1c0e-216">едукатионалактивитиес</span><span class="sxs-lookup"><span data-stu-id="f1c0e-216">educationalActivities</span></span>  |<span data-ttu-id="f1c0e-217">Коллекция [едукатионалактивити](educationalactivity.md)</span><span class="sxs-lookup"><span data-stu-id="f1c0e-217">[educationalActivity](educationalactivity.md) collection</span></span>      | <span data-ttu-id="f1c0e-218">Представляет данные, которые пользователь предоставил, относящихся к выпуску, выпускнику, выпуску или другим учебным действиям.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-218">Represents data that a user has supplied related to undergraduate, graduate, postgraduate or other educational activities.</span></span> <span data-ttu-id="f1c0e-219">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-219">Read-only.</span></span> <span data-ttu-id="f1c0e-220">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-220">Nullable.</span></span>|
|<span data-ttu-id="f1c0e-221">письма</span><span class="sxs-lookup"><span data-stu-id="f1c0e-221">emails</span></span>                 |<span data-ttu-id="f1c0e-222">Коллекция [итемемаил](itememail.md)</span><span class="sxs-lookup"><span data-stu-id="f1c0e-222">[itemEmail](itememail.md) collection</span></span>                          | <span data-ttu-id="f1c0e-223">Представляет подробные сведения об адресах электронной почты, связанных с пользователем.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-223">Represents detailed information about email addresses associated with the user.</span></span> <span data-ttu-id="f1c0e-224">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-224">Read-only.</span></span> <span data-ttu-id="f1c0e-225">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-225">Nullable.</span></span>|
|<span data-ttu-id="f1c0e-226">interests;</span><span class="sxs-lookup"><span data-stu-id="f1c0e-226">interests</span></span>              |<span data-ttu-id="f1c0e-227">Коллекция [персонинтерест](personinterest.md)</span><span class="sxs-lookup"><span data-stu-id="f1c0e-227">[personInterest](personinterest.md) collection</span></span>                | <span data-ttu-id="f1c0e-228">Предоставляет подробные сведения о интересах, которые пользователь связал с собственными службами в различных службах.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-228">Provides detailed information about interests the user has associated with themselves in various services.</span></span> <span data-ttu-id="f1c0e-229">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-229">Read-only.</span></span> <span data-ttu-id="f1c0e-230">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-230">Nullable.</span></span>|
|<span data-ttu-id="f1c0e-231">Языки</span><span class="sxs-lookup"><span data-stu-id="f1c0e-231">languages</span></span>              |<span data-ttu-id="f1c0e-232">Коллекция [лангуажепрофиЦиенци](languageproficiency.md)</span><span class="sxs-lookup"><span data-stu-id="f1c0e-232">[languageProficiency](languageproficiency.md) collection</span></span>      | <span data-ttu-id="f1c0e-233">Представляет подробные сведения о языках, добавленных пользователем в свой профиль.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-233">Represents detailed information about languages that a user has added to their profile.</span></span> <span data-ttu-id="f1c0e-234">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-234">Read-only.</span></span> <span data-ttu-id="f1c0e-235">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-235">Nullable.</span></span>|
|<span data-ttu-id="f1c0e-236">phones</span><span class="sxs-lookup"><span data-stu-id="f1c0e-236">phones</span></span>                 |<span data-ttu-id="f1c0e-237">Коллекция [итемфоне](itemphone.md)</span><span class="sxs-lookup"><span data-stu-id="f1c0e-237">[itemPhone](itemphone.md) collection</span></span>                          | <span data-ttu-id="f1c0e-238">Представляет подробные сведения о номерах телефонов, связанных с пользователем в различных службах.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-238">Represents detailed information about phone numbers associated with a user in various services.</span></span> <span data-ttu-id="f1c0e-239">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-239">Read-only.</span></span> <span data-ttu-id="f1c0e-240">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-240">Nullable.</span></span>|
|<span data-ttu-id="f1c0e-241">расположен</span><span class="sxs-lookup"><span data-stu-id="f1c0e-241">positions</span></span>              |<span data-ttu-id="f1c0e-242">Коллекция [воркпоситион](workposition.md)</span><span class="sxs-lookup"><span data-stu-id="f1c0e-242">[workPosition](workposition.md) collection</span></span>                    | <span data-ttu-id="f1c0e-243">Представляет подробные сведения о должностных единицах, связанных с профилем пользователя.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-243">Represents detailed information about work positions associated with a user's profile.</span></span> <span data-ttu-id="f1c0e-244">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-244">Read-only.</span></span> <span data-ttu-id="f1c0e-245">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-245">Nullable.</span></span>|
|<span data-ttu-id="f1c0e-246">projects</span><span class="sxs-lookup"><span data-stu-id="f1c0e-246">projects</span></span>               |<span data-ttu-id="f1c0e-247">Коллекция [прожектпартиЦипатион](projectparticipation.md)</span><span class="sxs-lookup"><span data-stu-id="f1c0e-247">[projectParticipation](projectparticipation.md) collection</span></span>    | <span data-ttu-id="f1c0e-248">Представляет подробные сведения о проектах, связанных с пользователем.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-248">Represents detailed information about projects associated with a user.</span></span> <span data-ttu-id="f1c0e-249">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-249">Read-only.</span></span> <span data-ttu-id="f1c0e-250">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-250">Nullable.</span></span>|
|<span data-ttu-id="f1c0e-251">skills.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-251">skills</span></span>                 |<span data-ttu-id="f1c0e-252">Коллекция [скиллпрофиЦиенци](skillproficiency.md)</span><span class="sxs-lookup"><span data-stu-id="f1c0e-252">[skillProficiency](skillproficiency.md) collection</span></span>            | <span data-ttu-id="f1c0e-253">Представляет подробные сведения о навыках, связанных с пользователем в различных службах.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-253">Represents detailed information about skills associated with a user in various services.</span></span> <span data-ttu-id="f1c0e-254">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-254">Read-only.</span></span> <span data-ttu-id="f1c0e-255">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-255">Nullable.</span></span>|
|<span data-ttu-id="f1c0e-256">Учетные записи учетных записей</span><span class="sxs-lookup"><span data-stu-id="f1c0e-256">webAccounts</span></span>            |<span data-ttu-id="f1c0e-257">Коллекция [учетных записей](webaccount.md)</span><span class="sxs-lookup"><span data-stu-id="f1c0e-257">[webAccount](webaccount.md) collection</span></span>                        | <span data-ttu-id="f1c0e-258">Представляет веб-учетные записи, которые пользователь указал, используют или добавили в свой профиль пользователя.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-258">Represents web accounts the user has indicated they use or has added to their user profile.</span></span> <span data-ttu-id="f1c0e-259">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-259">Read-only.</span></span> <span data-ttu-id="f1c0e-260">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-260">Nullable.</span></span>|
|<span data-ttu-id="f1c0e-261">websites</span><span class="sxs-lookup"><span data-stu-id="f1c0e-261">websites</span></span>               |<span data-ttu-id="f1c0e-262">Коллекция [персонвебсите](personwebsite.md)</span><span class="sxs-lookup"><span data-stu-id="f1c0e-262">[personWebsite](personwebsite.md) collection</span></span>                  | <span data-ttu-id="f1c0e-263">Представляет подробные сведения о веб-сайтах, связанных с пользователем в различных службах.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-263">Represents detailed information about websites associated with a user in various services.</span></span> <span data-ttu-id="f1c0e-264">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-264">Read-only.</span></span> <span data-ttu-id="f1c0e-265">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-265">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f1c0e-266">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f1c0e-266">JSON representation</span></span>

<span data-ttu-id="f1c0e-267">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1c0e-267">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.profile",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
    "id": "profileId",
    "anniversaries": [],
    "websites": [],
    "educationalActivities": [
        {
            "endMonthYear": null,
            "startMonthYear": null,
            "completionMonthYear": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "c3a9f515-4a15-456b-9bf7-690dcd7f05d7",
            "program": {
                "abbreviation": null,
                "description": null,
                "displayName": "",
                "grade": null,
                "notes": null,
                "webUrl": null
            },
            "institution": {
                "description": null,
                "displayName": "Colorado State University",
                "location": null,
                "webUrl": null
            },
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "emails": [
        {
            "address": "john.doe@contoso.com",
            "displayName": null,
            "type": "main",
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "046452c0-c893-4fd1-a7ca-57e2ccf13861",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "interests": [
        {
            "categories": [],
            "description": null,
            "displayName": "Microsoft Graph",
            "webUrl": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "0c568cf5-5e44-4b3e-aefd-6b46ca00a880",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "languages": [
        {
            "displayName": "English (United States)",
            "tag": "en-US",
            "proficiency": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "3d34dc2e-fc84-43ff-98f6-884467caba72",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],

    "names": [
        {
            "displayName": "John Doe",
            "first": "John",
            "initials": "JD",
            "last": "Doe",
            "languageTag": null,
            "maiden": null,
            "middle": null,
            "nickname": null,
            "suffix": null,
            "title": null,
            "pronunciation": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "b79302ca-7f05-4c89-96ce-b89d5855eb0e",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "phones": [
        {
            "displayName": null,
            "type": "business",
            "number": "+47 (9) 387654321",
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "d22aef2c-f332-4958-aac3-8d1d710a9e32",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "positions": [
        {
            "categories": [],
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "0f4d49c8-76cb-4d56-9f92-a10e182ba0e1",
            "detail": {
                "description": null,
                "endMonthYear": "0001-01-01",
                "jobTitle": "Associate Architect",
                "startMonthYear": "0001-01-01",
                "summary": null,
                "company": {
                    "displayName": "Contoso Corporation",
                    "pronunciation": null,
                    "department": "Architecture",
                    "officeLocation": "",
                    "webUrl": null,
                    "address": {
                        "type": "business",
                        "postOfficeBox": null,
                        "street": "",
                        "city": "Oslo",
                        "state": "",
                        "countryOrRegion": "",
                        "postalCode": ""
                    }
                }
            },
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "projects": [
        {
            "categories": [],
            "client": null,
            "displayName": "Profile on Graph",
            "detail": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "d6d84567-513a-47be-9be2-99fee6a12777",
            "colleagues": [],
            "sponsors": [],
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "skills": [
        {
            "categories": [],
            "displayName": "REST API Design",
            "proficiency": null,
            "webUrl": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "9cd979f9-7a43-4dd1-a628-42bb07bd0974",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "webAccounts": []
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: тип перечисления Кэйсторажепровидероптион
description: Параметры импорта поставщика хранилища ключей (KSP).
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 21a2e72bc226fdd7a965fbfb3f6ddd7735a4f351
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325507"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="1b7a1-103">тип перечисления Кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="1b7a1-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="1b7a1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b7a1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b7a1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1b7a1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b7a1-106">Параметры импорта поставщика хранилища ключей (KSP).</span><span class="sxs-lookup"><span data-stu-id="1b7a1-106">Key Storage Provider (KSP) Import Options.</span></span>

## <a name="members"></a><span data-ttu-id="1b7a1-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="1b7a1-107">Members</span></span>
|<span data-ttu-id="1b7a1-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="1b7a1-108">Member</span></span>|<span data-ttu-id="1b7a1-109">Значение</span><span class="sxs-lookup"><span data-stu-id="1b7a1-109">Value</span></span>|<span data-ttu-id="1b7a1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1b7a1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b7a1-111">усетпмкспосервисеусесофтварексп</span><span class="sxs-lookup"><span data-stu-id="1b7a1-111">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="1b7a1-112">нуль</span><span class="sxs-lookup"><span data-stu-id="1b7a1-112">0</span></span>|<span data-ttu-id="1b7a1-113">Импорт в KSP доверенного платформенного модуля (TPM), если он присутствует, в противном случае импортировать в KSP программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="1b7a1-113">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="1b7a1-114">усетпмкспосервисефаил</span><span class="sxs-lookup"><span data-stu-id="1b7a1-114">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="1b7a1-115">1,1</span><span class="sxs-lookup"><span data-stu-id="1b7a1-115">1</span></span>|<span data-ttu-id="1b7a1-116">Импорт в KSP доверенного платформенного модуля (TPM), если он присутствует, в противном случае произойдет ошибка.</span><span class="sxs-lookup"><span data-stu-id="1b7a1-116">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="1b7a1-117">усепасспортфорворккспосервисефаил</span><span class="sxs-lookup"><span data-stu-id="1b7a1-117">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="1b7a1-118">2</span><span class="sxs-lookup"><span data-stu-id="1b7a1-118">2</span></span>|<span data-ttu-id="1b7a1-119">Импорт в паспорт для Works KSP, если он доступен, в противном случае произойдет ошибка.</span><span class="sxs-lookup"><span data-stu-id="1b7a1-119">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="1b7a1-120">усесофтварексп</span><span class="sxs-lookup"><span data-stu-id="1b7a1-120">useSoftwareKsp</span></span>|<span data-ttu-id="1b7a1-121">4</span><span class="sxs-lookup"><span data-stu-id="1b7a1-121">3</span></span>|<span data-ttu-id="1b7a1-122">Импорт в KSP программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="1b7a1-122">Import to Software KSP.</span></span>|




---
title: Создание windowsPhone81AppX
description: Создание нового объекта windowsPhone81AppX.
ms.openlocfilehash: 13c2e2b0484b5760973a67dbb980bdf829c7ba32
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080151"
---
# <a name="create-windowsphone81appx"></a><span data-ttu-id="4e411-103">Создание windowsPhone81AppX</span><span class="sxs-lookup"><span data-stu-id="4e411-103">Create windowsPhone81AppX</span></span>

> <span data-ttu-id="4e411-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4e411-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e411-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e411-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4e411-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4e411-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4e411-107">Создание нового объекта [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) .</span><span class="sxs-lookup"><span data-stu-id="4e411-107">Create a new [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4e411-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4e411-108">Prerequisites</span></span>
<span data-ttu-id="4e411-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e411-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e411-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e411-111">Permission type</span></span>|<span data-ttu-id="4e411-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e411-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e411-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e411-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e411-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e411-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4e411-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e411-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e411-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e411-116">Not supported.</span></span>|
|<span data-ttu-id="4e411-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e411-117">Application</span></span>|<span data-ttu-id="4e411-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e411-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e411-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e411-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="4e411-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e411-120">Request headers</span></span>
|<span data-ttu-id="4e411-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4e411-121">Header</span></span>|<span data-ttu-id="4e411-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4e411-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e411-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e411-123">Authorization</span></span>|<span data-ttu-id="4e411-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4e411-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e411-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4e411-125">Accept</span></span>|<span data-ttu-id="4e411-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4e411-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e411-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4e411-127">Request body</span></span>
<span data-ttu-id="4e411-128">В тексте запроса укажите представление JSON для объекта windowsPhone81AppX.</span><span class="sxs-lookup"><span data-stu-id="4e411-128">In the request body, supply a JSON representation for the windowsPhone81AppX object.</span></span>

<span data-ttu-id="4e411-129">В следующей таблице показаны свойства, которые необходимы для создания windowsPhone81AppX.</span><span class="sxs-lookup"><span data-stu-id="4e411-129">The following table shows the properties that are required when you create the windowsPhone81AppX.</span></span>

|<span data-ttu-id="4e411-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e411-130">Property</span></span>|<span data-ttu-id="4e411-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4e411-131">Type</span></span>|<span data-ttu-id="4e411-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4e411-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e411-133">id</span><span class="sxs-lookup"><span data-stu-id="4e411-133">id</span></span>|<span data-ttu-id="4e411-134">String</span><span class="sxs-lookup"><span data-stu-id="4e411-134">String</span></span>|<span data-ttu-id="4e411-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4e411-135">Key of the entity.</span></span> <span data-ttu-id="4e411-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e411-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e411-137">displayName</span><span class="sxs-lookup"><span data-stu-id="4e411-137">displayName</span></span>|<span data-ttu-id="4e411-138">String</span><span class="sxs-lookup"><span data-stu-id="4e411-138">String</span></span>|<span data-ttu-id="4e411-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="4e411-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4e411-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e411-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e411-141">описание</span><span class="sxs-lookup"><span data-stu-id="4e411-141">description</span></span>|<span data-ttu-id="4e411-142">String</span><span class="sxs-lookup"><span data-stu-id="4e411-142">String</span></span>|<span data-ttu-id="4e411-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="4e411-143">The description of the app.</span></span> <span data-ttu-id="4e411-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e411-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e411-145">publisher</span><span class="sxs-lookup"><span data-stu-id="4e411-145">publisher</span></span>|<span data-ttu-id="4e411-146">String</span><span class="sxs-lookup"><span data-stu-id="4e411-146">String</span></span>|<span data-ttu-id="4e411-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="4e411-147">The publisher of the app.</span></span> <span data-ttu-id="4e411-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e411-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e411-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4e411-149">largeIcon</span></span>|[<span data-ttu-id="4e411-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4e411-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4e411-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="4e411-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4e411-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e411-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e411-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4e411-153">createdDateTime</span></span>|<span data-ttu-id="4e411-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e411-154">DateTimeOffset</span></span>|<span data-ttu-id="4e411-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="4e411-155">The date and time the app was created.</span></span> <span data-ttu-id="4e411-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e411-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e411-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4e411-157">lastModifiedDateTime</span></span>|<span data-ttu-id="4e411-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e411-158">DateTimeOffset</span></span>|<span data-ttu-id="4e411-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="4e411-159">The date and time the app was last modified.</span></span> <span data-ttu-id="4e411-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e411-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e411-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4e411-161">isFeatured</span></span>|<span data-ttu-id="4e411-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e411-162">Boolean</span></span>|<span data-ttu-id="4e411-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e411-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e411-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4e411-164">privacyInformationUrl</span></span>|<span data-ttu-id="4e411-165">String</span><span class="sxs-lookup"><span data-stu-id="4e411-165">String</span></span>|<span data-ttu-id="4e411-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="4e411-166">The privacy statement Url.</span></span> <span data-ttu-id="4e411-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e411-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e411-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4e411-168">informationUrl</span></span>|<span data-ttu-id="4e411-169">String</span><span class="sxs-lookup"><span data-stu-id="4e411-169">String</span></span>|<span data-ttu-id="4e411-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="4e411-170">The more information Url.</span></span> <span data-ttu-id="4e411-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e411-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e411-172">owner</span><span class="sxs-lookup"><span data-stu-id="4e411-172">owner</span></span>|<span data-ttu-id="4e411-173">String</span><span class="sxs-lookup"><span data-stu-id="4e411-173">String</span></span>|<span data-ttu-id="4e411-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="4e411-174">The owner of the app.</span></span> <span data-ttu-id="4e411-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e411-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e411-176">developer</span><span class="sxs-lookup"><span data-stu-id="4e411-176">developer</span></span>|<span data-ttu-id="4e411-177">String</span><span class="sxs-lookup"><span data-stu-id="4e411-177">String</span></span>|<span data-ttu-id="4e411-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="4e411-178">The developer of the app.</span></span> <span data-ttu-id="4e411-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e411-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e411-180">notes</span><span class="sxs-lookup"><span data-stu-id="4e411-180">notes</span></span>|<span data-ttu-id="4e411-181">String</span><span class="sxs-lookup"><span data-stu-id="4e411-181">String</span></span>|<span data-ttu-id="4e411-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="4e411-182">Notes for the app.</span></span> <span data-ttu-id="4e411-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e411-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e411-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="4e411-184">uploadState</span></span>|<span data-ttu-id="4e411-185">Int32</span><span class="sxs-lookup"><span data-stu-id="4e411-185">Int32</span></span>|<span data-ttu-id="4e411-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="4e411-186">The upload state.</span></span> <span data-ttu-id="4e411-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e411-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4e411-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="4e411-188">publishingState</span></span>|[<span data-ttu-id="4e411-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4e411-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4e411-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="4e411-190">The publishing state for the app.</span></span> <span data-ttu-id="4e411-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="4e411-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4e411-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e411-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="4e411-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="4e411-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4e411-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="4e411-194">committedContentVersion</span></span>|<span data-ttu-id="4e411-195">String</span><span class="sxs-lookup"><span data-stu-id="4e411-195">String</span></span>|<span data-ttu-id="4e411-196">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="4e411-196">The internal committed content version.</span></span> <span data-ttu-id="4e411-197">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e411-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="4e411-198">fileName</span><span class="sxs-lookup"><span data-stu-id="4e411-198">fileName</span></span>|<span data-ttu-id="4e411-199">String</span><span class="sxs-lookup"><span data-stu-id="4e411-199">String</span></span>|<span data-ttu-id="4e411-200">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="4e411-200">The name of the main Lob application file.</span></span> <span data-ttu-id="4e411-201">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e411-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="4e411-202">size</span><span class="sxs-lookup"><span data-stu-id="4e411-202">size</span></span>|<span data-ttu-id="4e411-203">Int64</span><span class="sxs-lookup"><span data-stu-id="4e411-203">Int64</span></span>|<span data-ttu-id="4e411-204">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="4e411-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="4e411-205">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e411-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="4e411-206">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="4e411-206">applicableArchitectures</span></span>|[<span data-ttu-id="4e411-207">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="4e411-207">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="4e411-208">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="4e411-208">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="4e411-209">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="4e411-209">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="4e411-210">identityName</span><span class="sxs-lookup"><span data-stu-id="4e411-210">identityName</span></span>|<span data-ttu-id="4e411-211">String</span><span class="sxs-lookup"><span data-stu-id="4e411-211">String</span></span>|<span data-ttu-id="4e411-212">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="4e411-212">The Identity Name.</span></span>|
|<span data-ttu-id="4e411-213">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="4e411-213">identityPublisherHash</span></span>|<span data-ttu-id="4e411-214">String</span><span class="sxs-lookup"><span data-stu-id="4e411-214">String</span></span>|<span data-ttu-id="4e411-215">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="4e411-215">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="4e411-216">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="4e411-216">identityResourceIdentifier</span></span>|<span data-ttu-id="4e411-217">String</span><span class="sxs-lookup"><span data-stu-id="4e411-217">String</span></span>|<span data-ttu-id="4e411-218">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="4e411-218">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="4e411-219">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4e411-219">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="4e411-220">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4e411-220">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="4e411-221">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="4e411-221">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="4e411-222">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="4e411-222">phoneProductIdentifier</span></span>|<span data-ttu-id="4e411-223">String</span><span class="sxs-lookup"><span data-stu-id="4e411-223">String</span></span>|<span data-ttu-id="4e411-224">Идентификатор продукта телефона.</span><span class="sxs-lookup"><span data-stu-id="4e411-224">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="4e411-225">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="4e411-225">phonePublisherId</span></span>|<span data-ttu-id="4e411-226">String</span><span class="sxs-lookup"><span data-stu-id="4e411-226">String</span></span>|<span data-ttu-id="4e411-227">Publisher с идентификатором телефона.</span><span class="sxs-lookup"><span data-stu-id="4e411-227">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="4e411-228">identityVersion</span><span class="sxs-lookup"><span data-stu-id="4e411-228">identityVersion</span></span>|<span data-ttu-id="4e411-229">String</span><span class="sxs-lookup"><span data-stu-id="4e411-229">String</span></span>|<span data-ttu-id="4e411-230">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="4e411-230">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="4e411-231">Ответ</span><span class="sxs-lookup"><span data-stu-id="4e411-231">Response</span></span>
<span data-ttu-id="4e411-232">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4e411-232">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e411-233">Пример</span><span class="sxs-lookup"><span data-stu-id="4e411-233">Example</span></span>
### <a name="request"></a><span data-ttu-id="4e411-234">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e411-234">Request</span></span>
<span data-ttu-id="4e411-235">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e411-235">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1419

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="4e411-236">Ответ</span><span class="sxs-lookup"><span data-stu-id="4e411-236">Response</span></span>
<span data-ttu-id="4e411-p121">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="4e411-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1527

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
  "id": "4ff27f80-7f80-4ff2-807f-f24f807ff24f",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```






---
title: Обработка событий, открытых Graph набор средств компонентов Майкрософт
description: Многие компоненты Graph набор средств Майкрософт выделяют настраиваемые события. Присоединение обработчиков событий к этим событиям позволяет отвечать на них и контролировать поведение приложения.
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: f20de269ed7f304f9c1d7198475b6fdb81b709c7
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082396"
---
# <a name="handle-events-exposed-by-microsoft-graph-toolkit-components"></a><span data-ttu-id="deb36-104">Обработка событий, открытых Graph набор средств компонентов Майкрософт</span><span class="sxs-lookup"><span data-stu-id="deb36-104">Handle events exposed by Microsoft Graph Toolkit components</span></span>

<span data-ttu-id="deb36-105">Многие компоненты Graph набор средств Майкрософт выделяют настраиваемые события.</span><span class="sxs-lookup"><span data-stu-id="deb36-105">Many Microsoft Graph Toolkit components emit custom events.</span></span> <span data-ttu-id="deb36-106">Присоединение обработчиков событий к этим событиям позволяет отвечать на них и контролировать поведение приложения.</span><span class="sxs-lookup"><span data-stu-id="deb36-106">Attaching event handlers to these events allows you to respond to them and control the behavior of your app.</span></span>

## <a name="discover-which-events-components-emit"></a><span data-ttu-id="deb36-107">Узнайте, какие компоненты событий выделяются</span><span class="sxs-lookup"><span data-stu-id="deb36-107">Discover which events components emit</span></span>

<span data-ttu-id="deb36-108">Каждый компонент Graph набор средств Майкрософт излучает различные события, определенные его функциональным возможностям.</span><span class="sxs-lookup"><span data-stu-id="deb36-108">Each Microsoft Graph Toolkit component emits different events, specific to its functionality.</span></span> <span data-ttu-id="deb36-109">Список событий, излучаемый конкретным компонентом, см. в разделе **События** документации по этому компоненту.</span><span class="sxs-lookup"><span data-stu-id="deb36-109">To see the list of events emitted by the specific component, see the **Events** section of the documentation for that component.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="deb36-110">Некоторые события, например в компоненте списка файлов, выделяются только `itemClick` при использовании шаблона по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="deb36-110">Some events, like `itemClick` in the File list component, are emitted only when using the default template.</span></span> <span data-ttu-id="deb36-111">При использовании настраиваемого шаблона переопишется отрисовка по умолчанию, отвечающего за излучение события.</span><span class="sxs-lookup"><span data-stu-id="deb36-111">If you use a custom template, you overwrite the default rendering that is responsible for emitting the event.</span></span>

## <a name="add-event-handlers-to-events"></a><span data-ttu-id="deb36-112">Добавление обработчиков событий в события</span><span class="sxs-lookup"><span data-stu-id="deb36-112">Add event handlers to events</span></span>

<span data-ttu-id="deb36-113">Корпорация Graph набор средств использует стандартную [`EventTarget.dispatchEvent()`](https://developer.mozilla.org/docs/Web/API/EventTarget/dispatchEvent) функцию для выпуска настраиваемого события в своих компонентах.</span><span class="sxs-lookup"><span data-stu-id="deb36-113">Microsoft Graph Toolkit uses the standard [`EventTarget.dispatchEvent()`](https://developer.mozilla.org/docs/Web/API/EventTarget/dispatchEvent) function to emit custom events in its components.</span></span> <span data-ttu-id="deb36-114">Чтобы прикрепить обработатель событий к настраиваемой событию, излучаемой компонентом инструментария, используйте стандартную [`EventTarget.addEventListener()`](https://developer.mozilla.org/docs/Web/API/EventTarget/addEventListener) функцию.</span><span class="sxs-lookup"><span data-stu-id="deb36-114">To attach an event handler to a custom event emitted by a toolkit's component, use the standard [`EventTarget.addEventListener()`](https://developer.mozilla.org/docs/Web/API/EventTarget/addEventListener) function.</span></span>

<span data-ttu-id="deb36-115">Например, для обработки события, излучаемого компонентом `itemClick` списка файлов, добавьте в код следующее.</span><span class="sxs-lookup"><span data-stu-id="deb36-115">For example, to handle the `itemClick` event emitted by the File list component, add the following to your code.</span></span>

```javascript
document.querySelector('mgt-file-list').addEventListener('itemClick' e => {
  // your event handler code goes here
});
```

### <a name="access-additional-information-exposed-by-the-event"></a><span data-ttu-id="deb36-116">Доступ к дополнительным сведениям, выставленным событием</span><span class="sxs-lookup"><span data-stu-id="deb36-116">Access additional information exposed by the event</span></span>

<span data-ttu-id="deb36-117">Некоторые события, излучаемые корпорацией Майкрософт Graph набор средств содержат дополнительные сведения, соответствующие событию.</span><span class="sxs-lookup"><span data-stu-id="deb36-117">Some events emitted by Microsoft Graph Toolkit contain additional information relevant to the event.</span></span> <span data-ttu-id="deb36-118">Например, событие, излучаемого компонентом списка файлов, содержит сведения о файле, который был нажат `itemClick` в списке файлов.</span><span class="sxs-lookup"><span data-stu-id="deb36-118">For example, the `itemClick` event, emitted by the File list component, contains information about the file that was clicked in the file list.</span></span> <span data-ttu-id="deb36-119">Дополнительные сведения см. в разделе **События** документации по соответствующему компоненту.</span><span class="sxs-lookup"><span data-stu-id="deb36-119">To see if the particular event contains additional information, see the **Events** section of the documentation for the corresponding component.</span></span>

<span data-ttu-id="deb36-120">Дополнительные сведения, открытые событием, можно получить с помощью свойства объекта, переданного в обработник событий, как показано `details` `event` в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="deb36-120">You can access the additional information exposed by an event through the `details` property of the `event` object passed into your event handler, as shown in the following example.</span></span>

```javascript
document.querySelector('mgt-file-list').addEventListener('itemClick', e => {
  const clickedFile = e.details;
});
```

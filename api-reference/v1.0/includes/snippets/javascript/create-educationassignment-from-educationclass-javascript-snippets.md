---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 60215b4cc8c5e410e02b5397649bd17ccffd2054
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2021
ms.locfileid: "60366071"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationAssignment = {
    dueDateTime: '2021-09-07T00:00:00Z',
    displayName: 'Reading test 09.03 #4',
    instructions: {
        contentType: 'text',
        content: 'Read chapter 4'
    },
    grading: {
        '@odata.type': '#microsoft.graph.educationAssignmentPointsGradeType',
        maxPoints: 50
    },
    assignTo: {
        '@odata.type': '#microsoft.graph.educationAssignmentClassRecipient'
    },
    status: 'draft',
    allowStudentsToAddResourcesToSubmission: true
};

await client.api('/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments')
    .post(educationAssignment);

```
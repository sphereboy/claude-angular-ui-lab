# Claude Angular UI Lab

This project demonstrates how to use Claude AI to assist in building and designing Angular UI components. It includes a workflow for designers and developers to collaborate effectively using Claude's capabilities.

## Project Overview

This project shows how to:
1. Set up an isolated Angular component development environment
2. Use Claude to generate and modify UI components
3. Test and preview components independently
4. Deploy components for review (e.g., to Netlify)

## Live Demo
Check out our example deployment: [Angular UI Components Demo](https://timely-dodol-7d26db.netlify.app/)

## Getting Started

### 1. Initial Setup
```bash
# Create a new Angular workspace without an application
ng new ui-components --create-application=false
cd ui-components

# Generate the component library
ng generate library design-system

# Create a demo application
ng generate application demo-app
```

### 2. Development Workflow

1. **Design Components**: Start with your design requirements
2. **Use Claude**: Ask Claude to help generate the component code
3. **Test & Review**: Use the demo app to test components
4. **Iterate**: Use Claude to refine and improve components

## Using Claude for UI Development

### Example Prompts

1. **Creating New Components**
```
Could you help me create an Angular component for [describe your component]?
```

2. **Modifying Existing Components**
```
I need to update this component to [describe changes]. Here's the current code: [paste code]
```

3. **Styling and Animations**
```
How can I add [describe animation/style] to this component?
```

### Best Practices

1. **Be Specific**: Provide detailed requirements
2. **Share Context**: Include relevant code snippets
3. **Iterate**: Break down complex components into smaller tasks
4. **Test Early**: Verify components in the demo app

## Project Structure

```
ui-components/
├── projects/
│   ├── design-system/        # Your component library
│   │   ├── src/
│   │   │   ├── lib/         # Components live here
│   │   │   └── public-api.ts
│   │   └── ng-package.json
│   └── demo-app/            